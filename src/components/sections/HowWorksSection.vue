<template>
  <div class="convideo">
    <h1 class="convideo__header">Как это работает</h1>
    <p class="convideo__description">Посмотрите краткий видеоурок, чтобы присоединиться к нам</p>
    <video
        @click="togglePlayPause"
        class="convideo__video"
        controls
        width="400"
        height="300"
        poster="/src/assets/img/video_banner.png"
    >
      <source
          src="https://videos.pexels.com/video-files/3571264/uhd_30fps.mp4"
          type="video/mp4"
      >
      <p>Your browser does not support the video tag.</p>
    </video>
  </div>
</template>

<script setup>
function togglePlayPause() {
  let video = document.querySelector('convideo__video');
  video.paused ? video.play() : video.pause()
}
</script>