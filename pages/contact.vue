<template>
  <section class="bg-[url('/assets/images/about-bg.svg')] bg-center bg-cover bg-no-repeat h-[50vh] flex items-center justify-center space-y-0  -mt-[50px]">
    <!-- <div class=" md:px-[10%] h-[inherit] items-center text-center"> -->
        <div class="">
            <h3 class="capitalize text-black font-bold text-[60px] font-frl  leading-[100%]">
                Contact Us
            </h3>
        </div>
     
    <!-- </div> -->
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

</script>

<style>

</style>
