<template>
  <q-carousel
    animated
    v-model="slide"
    arrows
    navigation
    infinite
    height="800px"
    :autoplay="autoplay"
  >
    <q-carousel-slide :name="1" img-src="img001.jpg" />
    <q-carousel-slide :name="2" img-src="img002.jpg" />
    <q-carousel-slide :name="3" img-src="img003.jpg" />
    <q-carousel-slide :name="4" img-src="img004.jpg" />
    <q-carousel-slide :name="5" img-src="img005.jpg" />
  </q-carousel>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const slide = ref(1);
const autoplay = ref(true);

defineOptions({
  name: 'IndexPage',
});
</script>
