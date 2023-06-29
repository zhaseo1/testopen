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
// new OpenInstall({
//   /*appKey必选参数，平台为每个应用分配的ID*/
//   appKey: "dpz2bf",
//   onready: function () {
    let downloadButton = document.querySelector(".downloadButton");
    downloadButton.addEventListener("click", function () {
      let fallbackLink = "https://down.ttiossign.com/#/join/6qWlf5";
      document.getElementById('loader').src = "dpz2bf://";
      fallbackLink = getOS() === "android" ? "https://metatravers.oss-cn-hongkong.aliyuncs.com/app-release.apk" :
          "https://down.ttiossign.com/#/join/6qWlf5";
      window.setTimeout(function () { window.location.replace(fallbackLink); }, 1);
    });
//   }
// });

function getOS() {
  const isiOS = /iPad|iPhone|iPod/.test(navigator.userAgent) && !window.MSStream;
  if (isiOS) return "ios";
  return "android";
}
</script>
