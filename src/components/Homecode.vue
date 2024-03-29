<template>
    <section class="flex flex-col lg:flex-center py-16 gap-6 sm:gap-10 md:gap-16 bg-gray-200">
      <!-- Photo - start -->
      <div class="text flex flex-col items-center text-center">
        <div class="lg:w-5/12 sm:text-center lg:py-12 lg:text-center xl:py-24">
          <p class="mb-4 font-semibold text-pink-600 md:mb-6 md:text-lg xl:text-xl">Project</p>
          <h1 class="mb-8 text-4xl font-bold text-purple-700 sm:text-5xl md:mb-12">Portfolio of Jazel Pangasi-an</h1>

          <div class="xl:w-7/12 flex justify-center items-center">
            <div class="img">
              <img src="https://scontent.fceb8-1.fna.fbcdn.net/v/t39.30808-1/434040729_791114996217412_8481271068723751192_n.jpg?stp=c0.0.320.320a_dst-jpg_p320x320&_nc_cat=103&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHzZ3dQ7scDBKg837gXYhBkgkq0DO2pF82CSrQM7akXzUhBGaJE3d4sn0KK3YJuiLJ6Xd_24fUF6GOfCOP6T3u2&_nc_ohc=cP-NKrIA8_QAX8M9EQH&_nc_oc=Adj_UuxWdOk3uA0JmjQCBhSMI48m_XsbURzkauRAWLT5pM36npAmi9rGh7YNaJKrreE&_nc_ht=scontent.fceb8-1.fna&oh=00_AfD_kMuvGIgfYLxFJrjE9VDhchJiuU9COHwvDIPiE8W62w&oe=6606BB74" alt="Photo of Jazel Pangasi-an" class="max-w-[150px] h-auto">
            </div>
          </div>
          <br>
          <br>


          <div class="flex gap-2.5 sm:flex-row sm:justify-center justify-center">
            <router-link to="/about" href="#" class="inline-block rounded-lg bg-pink-700 px-8 py-3 text-center text-sm font-semibold text-white outline-none ring-indigo-300 transition duration-100 hover:bg-pink-600 focus-visible:ring active:bg-pink-700 md:text-base">
              About Me
            </router-link>
            <router-link to="/contact" class="inline-block rounded-lg bg-gray-200 px-8 py-3 text-center text-sm font-semibold text-purple-500 outline-none ring-indigo-300 transition duration-100 hover:bg-violet-300 focus-visible:ring active:text-purple-700 md:text-base">
              Contact Me
            </router-link>
          </div>
        </div>
      </div>
    </section>
  </template>

  <style scoped>
  .img img {
    border-radius: 20px;
  }
  </style>
