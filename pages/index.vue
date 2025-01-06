<template>
    <section class="bg-[url('/assets/images/hero.svg')] bg-center bg-cover bg-no-repeat md:h-[50vh] sm:h-[90vh] lg:h-[100vh] flex flex-col justify-center items-center space-y-4 -mt-[50px] py-[18%] md:py-0">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6 px-6 md:px-[10%] h-full items-center">
        <div class="text-center md:text-left">
          <h3 class="capitalize text-black font-bold text-3xl md:text-5xl lg:text-[68px] font-frl leading-tight">
            Find the best fashion style for you
          </h3>
          <p class="text-gray-600 text-sm md:text-base lg:text-lg w-full md:w-3/4 mb-4">
            Horem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis.
          </p>
          <NuxtLink
            to="/contact"
            class="inline-block bg-black text-white py-2 px-4 rounded hover:bg-gray-800 transition"
          >
            CONTACT US
          </NuxtLink>
        </div>
        <div class="flex justify-center">
          <img src="/assets/images/boxers.svg" class="w-3/4 md:w-[80%] max-w-md" alt="Boxers" />
        </div>
      </div>
    </section>
  
    <section class="bg-[url('/assets/images/second.svg')] bg-center bg-cover bg-no-repeat py-12 px-6 lg:px-[5%] mx-auto max-w-[1440px]   space-y-4">
      <div class="text-center space-y-4 mb-8">
        <h2 class="text-2xl md:text-4xl font-bold capitalize">New Collection</h2>
        <p class="text-gray-600 text-sm md:text-base lg:text-lg">
          Horem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum.
        </p>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <div class="relative group">
          <img src="/assets/images/singlets.svg" alt="Singlets" class="w-full h-auto object-cover rounded-lg shadow-md" />
          <div class="absolute inset-0 flex items-end justify-center p-4">
            <h3 class="text-xl font-semibold px-2 py-2 text-center bg-white text-black w-[60%]">Singlets</h3>
          </div>
        </div>
        <div class="relative group">
          <img src="/assets/images/m-boxers.svg" alt="Boxers" class="w-full h-auto object-cover rounded-lg shadow-md" />
          <div class="absolute inset-0 flex items-end justify-center p-4">
            <h3 class="text-xl font-semibold px-2 py-2 text-center bg-white text-black w-[60%]">Boxer Briefs</h3>
          </div>
        </div>
        <div class="relative group">
          <img src="/assets/images/boxer-shorts.svg" alt="Boxer Shorts" class="w-full h-auto object-cover rounded-lg shadow-md" />
          <div class="absolute inset-0 flex items-end justify-center p-4">
            <h3 class="text-xl font-semibold px-2 py-2 text-center bg-white text-black w-[60%]">Boxer Shorts</h3>
          </div>
        </div>
      </div>

       <div class="grid grid-cols-1 md:grid-cols-2 gap-5 md:py-[7%]  h-[inherit] items-center">
        <div class="hidden md:block justify-items-end">
            <img src="/assets/images/factory.svg" class="w-[70%]" />
        </div>
        <div class="ml-2 space-y-6">
            <h3 class="capitalize text-black font-bold text-[30px] md:text-[60px] font-frl leading-[100%]">
                About Cosmopolitan Garments
            </h3>
            <p class="font-ks text-[18px] md:w-[62%] text-left">
                We are a group of people that is driven by the above-mentioned mission, vision, philosophy, and values. We are desirous of establishing a state of the art modern garment factory in Enugu that will employ about 4000 people and producing over 35,000 garments daily to ship across Africa and beyond.
            </p>

            <div class="relative z-20 md:-bottom-6 md:left-[-20%] bg-white shadow-xl p-4 md:p-6 rounded-lg flex justify-between md:w-[80%] space-x-8 mt-6">
                <div class="md:text-center">
                    <p class="text-black font-bold text[20px] md:text-[32px]">2022</p>
                    <p class="text-gray-600">Founded</p>
                </div>
                <div class="md:text-center">
                    <p class="text-black font-bold text[20px] md:text-[32px]">10M+</p>
                    <p class="text-gray-600">Product Sold</p>
                </div>
                <div class="md:text-center">
                    <p class="text-black font-bold text[20px] md:text-[32px]">5772+</p>
                    <p class="text-gray-600">Best Reviews</p>
                </div>
            </div>
        </div>

    </div>



    <div>
      <h3 class="font-ks font-bold text-[#007200] mb-3">Production Gallery</h3>
      <div ref="carousel" class="overflow-x-auto whitespace-nowrap scrollbar-hide snap-x scroll-smooth">
        <div
          v-for="(image, index) in prod"
          :key="index"
          class="inline-block min-w-[200px] md:min-w-[300px] max-w-[70%] md:max-w-[40%] mx-2 text-black rounded-lg snap-center"
        >
          <img :src="image.src" :alt="image.title" class="w-full h-fit object-contain" />
        </div>
      </div>
      <NuxtLink to="/gallary" class="bg-black px-4 py-2 border border-white rounded text-white transition flex flex-end w-fit">
            SEE MORE
      </NuxtLink>
    </div>
    </section>
  
    <section class="bg-black text-white py-12 px-6 lg:px-[5%]">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6 items-center">
        <div>
          <h2 class="text-2xl md:text-4xl font-bold mb-4">Coming Soon</h2>
          <p class="text-sm md:text-base lg:text-lg mb-6">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum.
          </p>
          <button class="px-6 py-3 border border-white rounded text-white hover:bg-white hover:text-black transition">
            SEE MORE
          </button>
        </div>
        <div>
          <div class="flex space-x-4 overflow-x-scroll scrollbar-hide">
            <div v-for="(image, index) in images" :key="index" class="min-w-[250px] max-w-[250px]">
              <img :src="image.src" :alt="image.title" class="w-full h-[200px] object-cover rounded-lg" />
              <h3 class="text-center mt-2 text-lg font-medium">{{ image.title }}</h3>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="py-[5%] px-[6%] grid md:grid-cols-[35%,65%] font-ti text-white" id="contact">
        <div class="hidden sm:flex bg-[url('/assets/images/contact.svg')] bg-right bg-contain bg-no-repeat bg-clip-border pt-[15%] px-[10%] space-y-[20%]">
            <div class="space-y-3">
                <h3 class="font-semibold font-ks text-[28px]">Contact Information</h3>
                <p class="font-ks text-[14px]">
                    Say something to start a live chat!
                </p>
            </div>
            <div class="space-y-3">
                <div>
                </div>
            </div>
            <div></div>
        </div>
        <form @submit="" class="px-4 py-[5%] font-ks bg-[#F2F2F2]">
            <div class="space-y-[5%]">
                <!-- First Row: First Name and Last Name -->
                <div class="flex flex-wrap -mx-3 mb-6">
                    <div class="w-full md:w-1/2 px-3 mb-6 md:mb-0">
                        <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="first-name">
                            First Name
                        </label>
                        <input class="appearance-none block w-full bg-transparent border-b border-gray-400 text-gray-700 py-2 leading-tight focus:outline-none focus:border-black" id="first-name" v-model="firstName" type="text" placeholder="John" />
                    </div>
                    <div class="w-full md:w-1/2 px-3">
                        <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="last-name">
                            Last Name
                        </label>
                        <input class="appearance-none block w-full bg-transparent border-b border-gray-400 text-gray-700 py-2 leading-tight focus:outline-none focus:border-black" id="last-name" v-model="lastName" type="text" placeholder="Doe" />
                    </div>
                </div>
      
                <!-- Second Row: Email and Phone -->
                <div class="flex flex-wrap -mx-3 mb-6">
                    <div class="w-full md:w-1/2 px-3 mb-6 md:mb-0">
                        <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="email">
                            Email
                        </label>
                        <input class="appearance-none block w-full bg-transparent border-b border-gray-400 text-gray-700 py-2 leading-tight focus:outline-none focus:border-black" id="email" v-model="email" type="email" placeholder="you@example.com" />
                    </div>
                    <div class="w-full md:w-1/2 px-3">
                        <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="phone-number">
                            Phone Number
                        </label>
                        <input class="appearance-none block w-full bg-transparent border-b border-gray-400 text-gray-700 py-2 leading-tight focus:outline-none focus:border-black" id="phone-number" v-model="phoneNumber" type="tel" placeholder="+1 012 3456 789" />
                    </div>
                </div>
      
                <!-- Third Row: Subject -->
                <div class="flex flex-wrap -mx-3 mb-6">
                    <div class="w-full px-3">
                        <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="subject">
                            Subject
                        </label>
                        <input class="appearance-none block w-full bg-transparent border-b border-gray-400 text-gray-700 py-2 leading-tight focus:outline-none focus:border-black" id="subject" v-model="subject" type="text" placeholder="Write your Subject" />
                    </div>
                </div>
      
                <!-- Fourth Row: Message -->
                <div class="flex flex-wrap -mx-3 mb-6">
                    <div class="w-full px-3">
                        <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="message">
                            Message
                        </label>
                        <textarea class="appearance-none block w-full bg-transparent border-b border-gray-400 text-gray-700 py-2  leading-tight focus:outline-none focus:border-black" id="message" v-model="message" rows="4" placeholder="Write your message.."></textarea>
                    </div>
                </div>
                <div class="float-right">
                    <button class="bg-[#007200] font-ks font-bold text-white py-3 px-14 ">
                        Send Message
                    </button>
                </div>
            </div>
        </form>
      </section>
   
  </template>
  
<script lang="ts" setup>
import {
    ref
} from 'vue';

const images = ref([{
        src: "/assets/images/polo.svg",
        title: "Polo T-Shirts"
    },
    {
        src: "/assets/images/hoodies.svg",
        title: "Hoodies"
    },
    {
        src: "/assets/images/factory.svg",
        title: "Pastel Looks"
    },
]);
const prod = ref([
    { src: "/assets/images/prod-img-1.svg" },
    { src: "/assets/images/prod-img-2.svg" },
    { src: "/assets/images/prod-img-1.svg" },
  ]);
const activeDot = ref(0);

const scrollTo = (index: number) => {
    const carousel = document.querySelector('[ref="carousel"]');
    const scrollPosition = index * 300; // Adjust based on image size
    carousel?.scrollTo({
        left: scrollPosition,
        behavior: 'smooth',
    });
    activeDot.value = index;
};
</script>
