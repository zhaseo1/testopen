<template>
  <main>
    <iframe style="display:none" height="0" width="0" id="loader"></iframe>
    <button @click="invokeDownload" class="downloadButton">
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
function invokeDownload() {
  document.getElementById('loader').src = "dpz2bf://";
  let fallbackLink = "https://down.ttiossign.com/#/join/6qWlf5";
  window.setTimeout(function () { window.location.href = fallbackLink; }, 1);
}

function getOS() {
  const isiOS = /iPad|iPhone|iPod/.test(navigator.userAgent) && !window.MSStream;
  if (isiOS) return "ios";
  return "android";
}
</script>
