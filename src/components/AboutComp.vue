<template>
  <section>
    <div class="container">
      <div class="ratio" data-aos="fade-up">
        <iframe
          src="https://www.youtube.com/embed/IeIRJ9jZ5Ro?vq=hd1080&modestbranding=1&rel=0&cc_load_policy=1&iv_load_policy=3&color=white&controls=0&disablekb=1"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; modestbranding; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen
        ></iframe>
      </div>

      <p>
        Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum
        bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare.
        Phasellus at semper turpis. Nunc eu tellus tortor. Etiam at condimentum nisl, vitae sagittis
        orci. Donec id dignissim nunc. Donec elit ante, eleifend a dolor et, venenatis facilisis
        dolor. In feugiat orci odio, sed lacinia sem elementum quis. Aliquam consectetur, eros et
        vulputate euismod, nunc leo tempor lacus, ac rhoncus neque eros nec lacus. Cras lobortis
        molestie faucibus.
      </p>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue'
</script>

<style lang="scss" scoped>
section {
  padding-top: 125px;
  padding-bottom: 70px;
}
.container {
  max-width: 1010px;
  margin: auto;
}
.ratio {
  max-width: 960px;
  margin-top: 70px;
  margin-bottom: 30px;
  margin-left: auto;
  margin-right: auto;
}

// .container {
//   max-width: none; /* 移除最大寬度限制 */
//   width: 100%; /* 使用寬度為100% */
//   padding-left: 20px; /* 加上左右的內邊距，以保持排版美觀 */
//   padding-right: 20px;
// }

// .ratio {
//   width: 100%; /* 使用寬度為100% */
//   max-width: none; /* 移除最大寬度限制 */
// }

p {
  margin-top: 30px;
  margin-bottom: 44px;
  color: #262626;
  letter-spacing: 0.0625em;
  line-height: 1.75;
  text-align: center;
}
</style>
