<template>
  <section class="bg-[url('/assets/images/about-bg.svg')] bg-center bg-cover bg-no-repeat h-[30vh] flex items-center justify-center space-y-0 -mt-[50px]">
    <div>
      <h3 class="capitalize text-black font-bold text-[60px] font-frl leading-[100%]">
        Production Gallery
      </h3>
    </div>
  </section>
  <section class="p-8 grid grid-cols-1 md:grid-cols-3 gap-6">
    <div
      v-for="(image, index) in images"
      :key="index"
      class="overflow-hidden rounded-lg shadow-lg"
    >
      <img
        :src="image.src"
        alt="Production image"
        class="w-full h-[400px] object-cover"
      />
    </div>
  </section>
</template>

<script lang="ts" setup>
const images = ref([
  { src: "/assets/images/prod-img-1.svg" },
  { src: "/assets/images/prod-img-2.svg" },
  { src: "/assets/images/prod-11.jpg" },
  { src: "/assets/images/prod-3.jpg" },
  { src: "/assets/images/prod-4.JPG" },
  { src: "/assets/images/prod-5.JPG" },
  { src: "/assets/images/prod-7.JPG" },
  { src: "/assets/images/prod-8.jpg" },
  { src: "/assets/images/prod-9.jpg" },
  { src: "/assets/images/prod-10.jpg" },
   { src: "/assets/images/prod-6.JPG" },
]);
</script>
