<template>
<footer class="w-full">
    <div class="hidden md:flex md:flex-row w-full ">
        <img src="/assets/images/footer-boxer1.svg" alt="Denham & Grey Logo" />
        <img src="/assets/images/footer-boxer2.svg" alt="Denham & Grey Logo" />
        <img src="/assets/images/footer-boxer3.svg" alt="Denham & Grey Logo" />
        <img src="/assets/images/footer-boxer4.svg" alt="Denham & Grey Logo" />
        <img src="/assets/images/footer-boxer5.svg" alt="Denham & Grey Logo" />
    </div>
    <div class="bg-black text-white text-center w-full space-y-[2%] h-[200px] items-center flex flex-col justify-center">
        <div class=" z-20 -top-6  bg-white shadow-xl p-6 rounded-lg  md:w-[30%]  -mt-[5%] capitalize text-black font-bold">
          FOLLOW OUR  INSTAGRAM: @xyz_abc
        </div>
        <div class="md:flex md:items-center md:justify-center space-x-6 text-white font-bold">
            <template v-for="(link, index) in menuItems" :key="index">
                <NuxtLink :to="link.path" @click="closeMenu" class="hover:text-primary-theme">
                    {{ link.name }}
                </NuxtLink>
            </template>
        </div>
        <p>Copyright {{currentYear}} COSMOPOLITAN GARMENTS, All Aight Reserved</p>
    </div>
</footer>
</template>

  
<script lang="ts" setup>
const currentYear = new Date().getFullYear();
const menuItems = ref([{
        name: 'Home',
        path: '/'
    },
    {
        name: 'Collection',
        path: '/'
    },
    {
        name: 'About Us',
        path: '/about'
    },
]);
</script>

  
<style scoped>
.text-white {
    color: #fff;
}

.text-gray-400 {
    color: #ccc;
}
</style>
