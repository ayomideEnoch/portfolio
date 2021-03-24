<template>
  <div
    class="min-h-screen w-full lg:px-24 md:px-12 px-4 pt-12"
    style="background-color: #151618"
  >
    <section class="flex justify-between text-gray-300">
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
    <div
      v-if="mobileMenu"
      class="bg-black z-10 fixed inset-0 w-full h-screen"
      style="background-color: #151618"
    >
      <div
        @click="mobileMenu = false"
        class="w-1/5 text-white cursor-pointer pt-10 pr-6 text-right text-2xl"
      >
        <i class="far fa-times"></i>
      </div>

      <div
        class="bg-white text-black w-4/5 h-screen z-20 fixed right-2 top-2 text-xl pt-8"
      >
        <!--  -->
        <div class="space-y-12 pl-6">
          <button class="block font-bold focus:outline-none">PORTFOLIO</button>
          <button class="block font-bold focus:outline-none">CONTACT</button>
          <button class="block font-bold focus:outline-none">ABOUT</button>
        </div>
      </div>
    </div>

    <section>
      <div class="mt-12 xl:mt-4">
        <!--  -->
        <div class="items-center lg:flex">
          <div class="">
            <img
              class="lg:rounded-full inset-0 object-cover lg:ml-44 ml-0 w-full"
              src="./assets/portfolio-man.jpg"
              alt=""
            />
          </div>
          <!--  -->
          <div class="text-gray-300 pr-0 xl:pr-28">
            <p
              class="xl:text-8xl lg:text-7xl md:text-7xl sm:text-6xl text-6xl font-bold xl:block flex justify-center"
            >
              CREATIVE
            </p>
            <p
              class="xl:text-7xl lg:text-6xl md:text-6xl sm:text-5xl text-5xl py-5 font-bold xl:block flex justify-center"
            >
              DEVELOPER
            </p>
            <p
              class="xl:text-4xl lg:text-3xl md:text-3xl sm:text-2xl text-2xl text-gray-500 font-normal flex justify-center"
            >
              SENSIBLE TO FRONTEND
            </p>
          </div>
          <div class="order-first lg:pt-0 pt-8">
            <div class="flex lg:block cursor-pointer items-center justify-center">
              <div
                class="text-xs font-semibold text-black bg-white rounded-full m-4 items-center justify-center w-4 flex h-4"
              >
                <i class="fab fa-facebook-f"></i>
              </div>

              <div
                class="text-xs font-semibold text-black bg-white rounded-full m-4 justify-center items-center w-4 flex h-4"
              >
                <i class="fab fa-twitter"></i>
              </div>

              <div
                class="text-xs font-semibold text-black bg-white rounded-full m-4 justify-center items-center w-4 flex h-4"
              >
                <i class="fab fa-github"></i>
              </div>

              <div
                class="text-xs font-semibold text-black bg-white rounded-full m-4 justify-center items-center w-4 flex h-4"
              >
                <i class="fab fa-linkedin-in"></i>
              </div>
            </div>
          </div>
        </div>

        <!--  -->
      </div>
    </section>
    <section
      class="flex justify-between text-gray-300 font-bold cursor-pointer xl:-mt-24 lg:-mt-1 md:-mt-6"
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
