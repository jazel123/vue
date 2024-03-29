<template>
    <MainLayout :pageTitle="pageTitle">
      <section class="flex flex-col justify-between min-h-screen">
        <div class="cont">
          <h1>Social Media</h1>
            <br>
            <br>
          <div class=" mt-8 flex flex-col items-center justify-center gap-4 sm:mt-16 lg:flex lg:justify-center">
            <div class="flex flex-col items-center">
              <span class="text-lg font-semibold uppercase tracking-widest text-purple-900 sm:text-base soc">Social</span>
              <span class="h-px w-12 bg-purple-200"></span>
            </div>
            <br><br>

            <div class="flex gap-8 items-center">
              <a :href="FacebookLink" target="_blank" class="flex items-center bg-blue text-blue-400 hover:text-blue-500 active:text-blue-600 ">
                <h6>FACEBOOK</h6>
                <svg class="h-10 w-10" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 8 19">
                  <path fill-rule="evenodd" d="M6.135 3H8V0H6.135a4.147 4.147 0 0 0-4.142 4.142V6H0v3h2v9.938h3V9h2.021l.592-3H5V3.591A.6.6 0 0 1 5.592 3h.543Z" clip-rule="evenodd" />
                </svg>
              </a>

              <a :href="InstagramLink" target="_blank" class="flex items-center bg-red text-red-400 hover:text-red-500 active:text-red-600 ">
                <h6>INSTAGRAM</h6>
                <svg class="h-10 w-10" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
                  <path fill="currentColor" d="M18 3H6C4.3 3 3 4.3 3 6v12c0 1.7 1.3 3 3 3h12c1.7 0 3-1.3 3-3V6c0-1.7-1.3-3-3-3m-6 6c1.7 0 3 1.3 3 3s-1.3 3-3 3s-3-1.3-3-3s1.3-3 3-3m3.8-2c0-.7.6-1.2 1.2-1.2s1.2.6 1.2 1.2s-.5 1.2-1.2 1.2s-1.2-.5-1.2-1.2M18 19H6c-.6 0-1-.4-1-1v-6h2c0 2.8 2.2 5 5 5s5-2.2 5-5h2v6c0 .6-.4 1-1 1"/></svg>
              </a>
            </div>
          </div>
        </div>
      </section>
    </MainLayout>
  </template>

  <script setup>
  import MainLayout from '../components/MainLayout.vue';

  // Social Links - Update this links to your link
  const FacebookLink = 'https://web.facebook.com/100059567566353';
  const InstagramLink = 'https://www.instagram.com/not_realaze?igsh=bmgxc3ZkZWt4eWx1';

  // Page Title of Views
  const pageTitle = 'Contact';
  </script>

  <style scoped>
  h1{
        color: black;
        font-size: 3rem;
        text-align: center;
          font-family: 'Times New Roman', Times, serif;

  }

  .cont {
    text-align: center;
  }

  /* Display flex for items to be aligned horizontally */
  .flex {
    display: flex;
  }
  </style>
