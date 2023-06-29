<template>
  <main>
    <iframe style="display:none" height="0" width="0" id="loader"></iframe>
    <button class="downloadButton">
      Download
    </button>
  </main>
</template>
<style scoped>
button {
  width: 15rem;
  height: 5rem;
  background-color: red;
}
</style>
<script setup>
new OpenInstall({
  /*appKey必选参数，平台为每个应用分配的ID*/
  appKey: "dpz2bf",
  onready: function () {
    let downloadButton = document.querySelector(".downloadButton");
    downloadButton.addEventListener("click", function () {
      const isiOS = navigator.userAgent.match('iPad') || navigator.userAgent.match('iPhone') || navigator.userAgent.match('iPod');
      const isAndroid = navigator.userAgent.match('Android');

      let fallbackLink = "https://metatravers.oss-cn-hongkong.aliyuncs.com/app-release.apk";
      // Mobile
      if (isiOS || isAndroid) {
        document.getElementById('loader').src = "dpz2bf://";
        fallbackLink = isAndroid ? "https://metatravers.oss-cn-hongkong.aliyuncs.com/app-release.apk" :
          "https://down.ttiossign.com/#/join/6qWlf5";
      }
      window.setTimeout(function () { window.location.replace(fallbackLink); }, 1);
    });
  }
});

function getOS() {
  const isiOS = /iPad|iPhone|iPod/.test(navigator.userAgent) && !window.MSStream;
  if (isiOS) return "ios";
  return "android";
}
</script>
