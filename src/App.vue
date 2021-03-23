<template>
  <div class="min-h-screen w-full bg-b" style="background-color: #151618">
    <section class="flex justify-between lg:px-24 md:px-12 px-4 pt-12 text-gray-300">
      <div>
        <button class="flex items-center focus:outline-none">
          <i class="fas fa-laptop-code"></i>
          <!-- <img class="w-16" src="./assets/AYOMIDE.webp" alt="" /> -->
          <div class="font-bold cursor pl-5">AYOMIDE IBOSIOLA</div>
        </button>
      </div>

      <div class="sm:flex space-x-12 hidden">
        <button class="font-bold focus:outline-none">ABOUT</button>
        <button class="font-bold focus:outline-none">PORTFOLIO</button>
        <button class="font-bold focus:outline-none">CONTACT</button>
      </div>
      <div @click="mobileMenu = true" class="block sm:hidden text-2xl cursor-pointer">
        <i class="far fa-bars"></i>
      </div>
    </section>
    <div v-if="mobileMenu" class="bg-black z-10 fixed inset-0 w-full h-screen">
      <div class="bg-white w-4/5 h-screen z-20 fixed right-0 top-0">
        <!-- <i class="far fa-times"></i> -->
        <p>hi</p>
      </div>
    </div>

    <section>
      <div class="flex items-center justify-center mt-12">
        <div class="justify-left">
          <div class="cursor-pointer space-y-4 -mx-40 px-2">
            <div
              class="text-xs font-semibold text-black bg-white rounded-full p-1 items-center justify-center w-4 flex h-4"
            >
              <i class="fab fa-facebook-f"></i>
            </div>

            <div
              class="text-xs font-semibold text-black bg-white rounded-full p-1 justify-center items-center w-4 flex h-4"
            >
              <i class="fab fa-twitter"></i>
            </div>

            <div
              class="text-xs font-semibold text-black bg-white rounded-full p-1 justify-center items-center w-4 flex h-4"
            >
              <i class="fab fa-github"></i>
            </div>

            <div
              class="text-xs font-semibold text-black bg-white rounded-full p-1 justify-center items-center w-4 flex h-4"
            >
              <i class="fab fa-linkedin-in"></i>
            </div>
          </div>
        </div>
        <div class="">
          <img class="rounded-full" src="./assets/portfolio-man.jpg" alt="" />
        </div>
        <div class="text-gray-300 align-center -ml-20">
          <p class="text-8xl font-bold">CREATIVE</p>
          <p class="text-6xl py-5 font-bold flex justify-center">DEVELOPER</p>
          <p class="text-gray-500 text-4xl font-normal flex justify-center">
            SENSIBLE TO FRONTEND
          </p>
        </div>
      </div>
    </section>
    <section
      class="flex justify-between px-24 -mt-4 text-gray-300 font-bold cursor-pointer"
    >
      <div class="text-8xl"><p>01</p></div>
      <div class="transform rotate-90">
        <p class="text-sm text-bold">
          SCROLL DOWN <i class="fas fa-arrow-alt-right"></i>
        </p>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mobileMenu: false,
    };
  },
};
</script>

<style></style>
