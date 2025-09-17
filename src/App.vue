<script setup>
import { Liquid } from '@antv/g2plot';
import { onMounted } from 'vue';

onMounted(() => {
  const liquidPlot = new Liquid('container', {
    percent: 0.25,
    outline: {
      border: 4,
      distance: 8,
    },
    wave: {
      length: 128,
    },
  });
  liquidPlot.render();
})
</script>
<template>
  <div class="content">
    <h1>Rsbuild with Vue</h1>
    <div id="container"></div>
  </div>
</template>

<style scoped>
.content {
  display: flex;
  min-height: 100vh;
  line-height: 1.1;
  text-align: center;
  flex-direction: column;
  justify-content: center;
}

.content h1 {
  font-size: 3.6rem;
  font-weight: 700;
}

.content p {
  font-size: 1.2rem;
  font-weight: 400;
  opacity: 0.5;
}
</style>
