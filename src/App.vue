<template>
  <div style="font-family: 'Roboto', sans-serif" class="">
    <section
      class="min-h-screen w-full lg:px-24 md:px-12 px-4 pt-12"
      style="background-color: #2d2e32"
    >
      <!-- Navbar -->
      <div class="flex justify-between text-gray-300">
        <div>
          <button class="flex items-center focus:outline-none">
            <i class="fas fa-laptop-code"></i>
            <div class="font-bold cursor pl-5">
              <span class="text-white">Ayòmídé</span> ÌBÒSÍOLÁ
            </div>
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
      </div>
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
      <!-- Navbar ends -->
      <div>
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
            <div class="order-first lg:pt-0 pt-8 flex lg:block justify-center">
              <a href="https://web.facebook.com/ayomide.ibosiola">
                <div class="flex lg:block cursor-pointer items-center justify-center">
                  <div
                    class="text-xs font-semibold text-black bg-white rounded-full m-4 items-center justify-center w-5 flex h-5"
                  >
                    <i class="fab fa-facebook-f"></i>
                  </div>
                </div>
              </a>
              <a href="https://twitter.com/ayomideIbosiola">
                <div class="flex lg:block cursor-pointer items-center justify-center">
                  <div
                    class="text-xs font-semibold text-black bg-white rounded-full m-4 justify-center items-center w-5 flex h-5"
                  >
                    <i class="fab fa-twitter"></i>
                  </div></div
              ></a>
              <a href="https://github.com/ayomideEnoch">
                <div class="flex lg:block cursor-pointer items-center justify-center">
                  <div
                    class="text-xs font-semibold text-black bg-white rounded-full m-4 justify-center items-center w-5 flex h-5"
                  >
                    <i class="fab fa-github"></i>
                  </div></div
              ></a>
              <a href="https://www.linkedin.com/in/ayomide-ibosiola/">
                <div class="flex lg:block cursor-pointer items-center justify-center">
                  <div
                    class="text-xs font-semibold text-black bg-white rounded-full m-4 justify-center items-center w-5 flex h-5"
                  >
                    <i class="fab fa-linkedin-in"></i>
                  </div></div
              ></a>
            </div>
          </div>
          <!--  -->
        </div>
      </div>
      <div class="lg:flex hidden justify-end cursor-pointer">
        <i class="text-gray-300 fal fa-arrow-down text-4xl animate-bounce"></i>
      </div>
    </section>

    <!-- About Me -->
    <section
      class="pb-16 min-h-screen w-full lg:px-24 md:px-12 px-4 pt-12"
      style="background-color: #252628"
    >
      <div class="font-semibold">
        <div class="flex items-center font-semibold">
          <i class="text-yellow-500 fas fa-hand-peace"></i>
          <p class="text-gray-500 pl-3">Welcome / Ẹ káàbọ̀</p>
        </div>
        <p class="text-gray-500 py-3 spacing text-3xl">My name is Ayomide Ibosiola.</p>
        <p class="text-white text-3xl">
          I'm a Nigerian Frontend Developer based in Ikosi-Ketu, Lagos state, Nigeria.
        </p>
        <div class="mt-8 sm:flex block">
          <div class="sm:w-6/12 w-full text-2xl text-white sm:mr-4 mr-0">
            <p>
              Interested in crafting
              <span class="text-gray-500">more cohesive </span> product experiences for
              humans
              <span class="text-gray-500">
                and design work holistically across a product.
              </span>
            </p>
            <p class="text-gray-500 text-sm py-7">
              That means potential research, visual and code.
            </p>
            <!-- About Me -->
            <div class="w-full border-b-2 border-yellow-300 mb-2"></div>
            <div>
              <p class="text-sm text-gray-500 font-semibold mb-2">MY SKILLS</p>

              <!--  -->
              <div class="flex flex-wrap w-full">
                <div
                  class="sm:w-1/2 w-full flex items-center mb-3"
                  v-for="skill in skills"
                  :key="skill.index"
                >
                  <div
                    class="sm:w-10 w-9 h-9 bg-gray-700 rounded-full flex items-center justify-center font-normal"
                  >
                    <i class="" :class="skill.icon"> </i>
                  </div>
                  <div class="ml-3 w-full">
                    <p class="text-base font-normal mb-2">
                      {{ skill.name }}
                    </p>
                    <div
                      class="h-2 sm:w-11/12 w-full relative rounded-full bg-gray-100 overflow-hidden"
                    >
                      <div
                        class="h-full absolute bg-green-500 rounded-full"
                        style=""
                        :style="{ width: skill.progress }"
                      ></div>
                    </div>
                  </div>
                </div>
              </div>

              <!--  -->
            </div>
          </div>
          <div class="w-1/12 mb-4"></div>
          <div class="sm:w-5/12 w-full">
            <p class="text-md text-white">Experience</p>
            <div class="pt-4">
              <div class="flex justify-between text-sm">
                <p class="text-white">Freelance</p>
                <p class="text-gray-500">2019 - Present</p>
              </div>
              <p class="text-gray-500 text-sm">Frontend Developer</p>
            </div>
            <div class="pt-4">
              <div class="flex justify-between text-sm">
                <p class="text-white">Royal Crystal Airways</p>
                <p class="text-gray-500">2020 - 2021</p>
              </div>
              <p class="text-gray-500 text-sm">Frontend Developer</p>
            </div>
            <div class="pt-4">
              <div class="flex justify-between text-sm">
                <p class="text-white">Midra Solutions</p>
                <p class="text-gray-500">2019 - 2020</p>
              </div>
              <p class="text-gray-500 text-sm">Frontend Developer</p>
            </div>

            <div class="pt-4">
              <div class="flex justify-between text-sm">
                <p class="text-white">Lagosbuild</p>
                <p class="text-gray-500">2017 - 2019</p>
              </div>
              <p class="text-gray-500 text-sm">Frontend Developer</p>
            </div>
            <div class="flex justify-between text-sm mt-10"></div>
          </div>
        </div>
      </div>
    </section>
    <section
      class="pb-5 min-h-screen w-full lg:px-24 md:px-12 px-4 pt-12"
      style="background-color: #191919"
    >
      <div class="">
        <p class="flex justify-center text-bold text-white text-4xl">Get in touch!</p>
        <p class="flex justify-center text-semibold text-gray-300 text-2xl pt-12 pb-24">
          For enquires, conferences, work or technical workshops.
        </p>
      </div>
      <div class="pb-24 flex justify-evenly text-gray-300 text-lg">
        <a
          href="https://www.google.com/maps/place/8+Kayode+Arikawe+St,+Ikosi+Ketu,+Lagos/data=!4m2!3m1!1s0x103b92fa4ecebf0f:0x5d279185dc75274?sa=X&ved=2ahUKEwjTvqCvttbvAhXFiVwKHW3mDmEQ8gEwAHoECAMQAQ"
          target="_blank"
        >
          <div
            class="p-4 space-y-4 hover:bg-gray-300 hover:text-black rounded-xl cursor-pointer"
          >
            <div class="text-center">
              <i class="fas fa-map-marker-alt text-3xl text-gray-600"></i>
              <p>8, Kayode Arikawe street, Ikosi-Ketu.</p>
            </div>
          </div>
        </a>
        <a href="tel:+2348099691225">
          <div
            class="p-4 space-y-4 hover:bg-gray-300 hover:text-black rounded-xl cursor-pointer"
          >
            <div class="text-center">
              <i class="fas fa-phone-alt text-3xl text-gray-600"></i>
              <p>+234 809 969 1225</p>
            </div>
          </div>
        </a>
        <a href="mailto:ayomideibosiola100@gmail.com">
          <div
            class="p-4 space-y-4 hover:bg-gray-300 hover:text-black rounded-xl cursor-pointer"
          >
            <div class="text-center">
              <i class="fas fa-envelope text-3xl text-gray-600"></i>
              <p>ayomideibosiola100@gmail.com</p>
            </div>
          </div>
        </a>
      </div>
      <div class="flex justify-center">
        <a href="https://web.facebook.com/ayomide.ibosiola">
          <div class="flex justify-center">
            <div
              class="text-2xl font-semibold text-black bg-white rounded-full m-4 items-center justify-center w-12 flex h-12"
            >
              <i class="fab fa-facebook-f"></i>
            </div>
          </div>
        </a>
        <a href="https://twitter.com/ayomideIbosiola">
          <div class="flex justify-center">
            <div
              class="text-2xl font-semibold text-black bg-white rounded-full m-4 justify-center items-center w-12 flex h-12"
            >
              <i class="fab fa-twitter"></i>
            </div>
          </div>
        </a>
        <a href="https://github.com/ayomideEnoch">
          <div class="flex justify-center">
            <div
              class="text-2xl font-semibold text-black bg-white rounded-full m-4 justify-center items-center w-12 flex h-12"
            >
              <i class="fab fa-github"></i>
            </div>
          </div>
        </a>

        <a href="https://www.linkedin.com/in/ayomide-ibosiola/">
          <div class="flex justify-center">
            <div
              class="text-2xl font-semibold text-black bg-white rounded-full m-4 justify-center items-center w-12 flex h-12"
            >
              <i class="fab fa-linkedin-in"></i>
            </div>
          </div>
        </a>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mobileMenu: false,
      skills: [
        {
          name: "VueJS",
          icon: "fab fa-vuejs text-green-500",
          progress: "90%",
        },
        {
          name: "ReactJS",
          icon: "fab fa-react text-blue-500",
          progress: "60%",
        },
        {
          name: "JavaScript",
          icon: "fab fa-js text-yellow-300",
          progress: "75%",
        },
        {
          name: "HTML",
          icon: "fab fa-html5 text-red-600",
          progress: "95%",
        },
        {
          name: "CSS",
          icon: "fab fa-css3-alt text-blue-500",
          progress: "90%",
        },
        {
          name: "Tailwind CSS",
          icon: "fas fa-code text-base",
          progress: "95%",
        },
        {
          name: "Bootstrap",
          icon: "fab fa-bootstrap text-purple-400",
          progress: "90%",
        },
        {
          name: "Material UI",
          icon: "fas fa-code text-base",
          progress: "70%",
        },
      ],
    };
  },
};
</script>

<style></style>
