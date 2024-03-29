<template>
    <header class="border-b border-gray-200 flex items-center justify-between h-24 w-full bg-black text-white">
      <!-- Philippine Logo -->
      <img :src="require('@/assets/cpc.png')" alt="CPC Logo" class="h-auto max-h-full w-auto max-w-full ml-4">

      <!-- Text: College of Technology Studies -->
      <p class="text-lg font-semibold">BSIT-College of Technology Studies</p>

      <nav class="px-12 py-4 flex flex-row items-center justify-between">
        <!-- Desktop Menu -->
        <div class="hidden lg:block items-center justify-between">
          <ul class="flex flex-row gap-8">
            <li
              :class="$route.name === 'home' ? 'bg-gray-50 p-2 rounded text-purple-700 font-medium text-lg' : 'hover:bg-purple-50 p-2 text-purple-700 hover:text-purple-700 font-normal text-lg'">
              <router-link to="/">Home</router-link>
            </li>
            <li
              :class="$route.name === 'about' ? 'bg-gray-50 p-2 rounded text-purple-700 font-medium text-lg' : 'hover:bg-purple-50 p-2 text-purple-700 hover:text-purple-700 font-normal text-lg'">
              <router-link to="/about">About</router-link>
            </li>
            <li
              :class="$route.name === 'contact' ? 'bg-gray-50 p-2 rounded text-purple-700 font-medium text-lg' : 'hover:bg-purple-50 p-2 text-purple-700 hover:text-purple-700 font-normal text-lg'">
              <router-link to="/contact">Contact</router-link>
            </li>
            <li
              :class="$route.name === 'skill' ? 'bg-gray-50 p-2 rounded text-purple-700 font-medium text-lg' : 'hover:bg-purple-50 p-2 text-purple-700 hover:text-purple-700 font-normal text-lg'">
              <router-link to="/skill">Skill</router-link>
            </li>
          </ul>
        </div>

        <!-- Burger Menu -->
        <div @click="toggleMobileMenu"
          class="cursor-pointer block lg:hidden border border-gray-200 bg-gray-100 hover:bg-gray-200 p-2 rounded-full">
          <svg class="w-[24px] h-[24px] text-gray-700" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 16 12">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"
              d="M1 1h14M1 6h14M1 11h7" />
          </svg>
        </div>

        <!-- Mobile Menu -->
        <div v-if="isOpenMenu" class=" flex lg:hidden relative">
          <div class="bg-white flex flex-col absolute top-[18px] -left-[52px] w-screen gap-4 shadow-lg p-6 rounded">
            <router-link to="/"
              :class="$route.name === 'home' ? 'bg-gray-50 p-2 rounded text-pink-700 font-medium text-lg' : 'hover:bg-pink-50 p-2 text-pink-700 hover:text-pink-700 font-normal text-lg'">
              Home
            </router-link>
            <router-link to="/about"
              :class="$route.name === 'about' ? 'bg-gray-50 p-2 rounded text-pink-700 font-medium text-lg' : 'hover:bg-pink-50 p-2 text-pink-700 hover:text-pink-700 font-normal text-lg'">
              About
            </router-link>
            <router-link to="/contact"
              :class="$route.name === 'contact' ? 'bg-gray-50 p-2 rounded text-pink-700 font-medium text-lg' : 'hover:bg-pink-50 p-2 text-pink-700 hover:text-pink-700 font-normal text-lg'">
              Contact
            </router-link>
            <router-link to="/skill"
              :class="$route.name === 'skill' ? 'bg-gray-50 p-2 rounded text-pink-700 font-medium text-lg' : 'hover:bg-pink-50 p-2 text-pink-700 hover:text-pink-700 font-normal text-lg'">
              Skill
            </router-link>
          </div>
        </div>
      </nav>
    </header>
</template>

<script setup>
import { ref } from 'vue';

const isOpenMenu = ref(false);

const toggleMobileMenu = () => {
  return isOpenMenu.value = !isOpenMenu.value;
};
</script>


