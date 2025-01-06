<template>
    <section class="bg-[url('/assets/images/about-bg.svg')] bg-center bg-cover bg-no-repeat py-[18%] md:h-[50vh] lg:h-[60vh] flex items-center justify-center -mt-[50px]">
      <div class="grid grid-cols-1 lg:grid-cols-[60%,40%] gap-6 md:px-[10%] h-full items-center">
        <div>
          <h3 class="capitalize text-black font-bold text-[36px] md:text-[48px] lg:text-[60px] font-frl leading-tight">
            Collection
          </h3>
        </div>
        <div>
          <img src="/assets/images/boxers.svg" class="w-[80%] lg:w-[65%] mx-auto" />
        </div>
      </div>
    </section>
  
    <section class="bg-[url('/assets/images/about-second.svg')] bg-center bg-cover bg-no-repeat py-8 px-4 md:px-[10%] lg:px-[15%]">
      <div class="space-y-8">
        <!-- Vision -->
        <div class="grid grid-cols-1 md:grid-cols-[15%,85%] gap-4">
          <div>
            <h3 class="font-ks font-bold text-[#007200]">Our Vision</h3>
          </div>
          <p class="font-ks font-semibold text-[14px] md:text-[16px]">
            Envisioning a continent where every individual experiences the joy of wearing garments that seamlessly blend quality, cultural acceptance, and affordability.
            <br /><br />
            Our vision is to establish a garment factory as the foremost symbol of garment excellence, setting the industry standard and contributing to Africa's socio-economic development through our commitment to quality and inclusivity.
          </p>
        </div>
  
        <!-- Mission -->
        <div class="grid grid-cols-1 md:grid-cols-[15%,85%] gap-4">
          <div>
            <h3 class="font-ks font-bold text-[#007200]">Our Mission</h3>
          </div>
          <p class="font-ks font-semibold text-[14px] md:text-[16px]">
            Envisioning a continent where every individual experiences the joy of wearing garments that seamlessly blend quality, cultural acceptance, and affordability.
            <br /><br />
            Our vision is to establish a garment factory as the foremost symbol of garment excellence, setting the industry standard and contributing to Africa's socio-economic development through our commitment to quality and inclusivity.
          </p>
        </div>
  
        <!-- Production Gallery -->
        <div>
          <h3 class="font-ks font-bold text-[#007200] mb-3">Production Gallery</h3>
          <div ref="carousel" class="overflow-x-auto whitespace-nowrap scrollbar-hide snap-x scroll-smooth">
            <div
              v-for="(image, index) in images"
              :key="index"
              class="inline-block min-w-[200px] md:min-w-[300px] max-w-[70%] md:max-w-[40%] mx-2 text-black rounded-lg snap-center"
            >
              <img :src="image.src" :alt="image.title" class="w-full h-fit object-contain" />
            </div>
            <NuxtLink to="/" class="relative inline-flex bg-gradient-to-r from-[#ffffffde] to-[#ffffff] h-[270px] left-[-31%]">
              <img src="/assets/images/arrow.svg" class="w-[20%]" />
            </NuxtLink>
          </div>
        </div>
  
        <!-- Philosophy -->
        <div class="grid grid-cols-1 md:grid-cols-[15%,85%] gap-4">
          <div>
            <h3 class="font-ks font-bold text-[#007200]">Our Philosophy</h3>
          </div>
          <p class="font-ks font-semibold text-[14px] md:text-[16px]">
            We uphold a philosophy rooted in the pursuit of precision in garment manufacturing. Our values embrace diversity, ensuring that our garments fit flawlessly and respect African cultures.
            <br /><br />
            We are committed to transparency, sustainability, and fostering a collaborative and empowering environment for our team.
            <br /><br />
            We are a group of people driven by the above-mentioned mission, vision, philosophy, and values. We are desirous of establishing a state-of-the-art modern garment factory in Enugu that will employ about 4000 people and produce over 35,000 garments daily to ship across Africa and beyond.
          </p>
        </div>
      </div>
    </section>
  
    <!-- Meet Our Team -->
    <section class="px-4 md:px-[10%] lg:px-[15%] py-8">
      <div>
        <h3 class="font-ks font-bold text-[#007200]">Meet Our Team</h3>
      </div>
      <div class="space-y-6 mt-6">
        <div class="grid grid-cols-1 md:grid-cols-3 md:gap-6">
          <div class="space-y-6 mb-4">
            <img src="/assets/images/ogb.svg" alt="Team Member 1" class="w-full object-cover rounded" />
            <img src="/assets/images/girl2.svg" alt="Team Member 2" class="hidden md:block w-full object-cover rounded" />
            <img src="/assets/images/kkb.svg" alt="Team Member 3" class="md:hidden w-full object-cover rounded" />
          </div>
          <div class="col-span-2 grid grid-cols-2 gap-4">
            <img src="/assets/images/kkb.svg" alt="Team Member 3" class="hidden md:block w-full object-cover rounded" />
            <img src="/assets/images/girl2.svg" alt="Team Member 2" class="md:hidden w-full object-cover rounded" />
            <img src="/assets/images/girl1.svg" alt="Team Member 4" class="w-full object-cover rounded" />
            <img src="/assets/images/team1.svg" alt="Team Group 1" class="col-span-2 w-full object-cover rounded" />
          </div>
        </div>
        <div>
          <img src="/assets/images/team2.svg" alt="Team Group 2" class="w-full object-contain rounded" />
        </div>
      </div>
    </section>
  </template>
  
  <script lang="ts" setup>
  const images = ref([
    { src: "/assets/images/prod-img-1.svg" },
    { src: "/assets/images/prod-img-2.svg" },
    { src: "/assets/images/prod-img-1.svg" },
  ]);
  </script>
  