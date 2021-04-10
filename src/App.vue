<template>
  <div style="font-family: 'Roboto', sans-serif" class="">
    <section
      class="min-h-screen w-full lg:px-24 md:px-12 px-4 pt-12"
      style="background-color: #2d2e32"
    >
      <!-- Navbar -->
      <div class="flex justify-between text-gray-300">
        <div>
          <a href="/">
            <button class="flex items-center focus:outline-none">
              <i class="fas fa-laptop-code"></i>
              <div class="font-bold cursor pl-5">
                <span class="text-white">Ayòmídé</span> ÌBÒSÍOLÁ
              </div>
            </button>
          </a>
        </div>

        <div class="sm:flex space-x-12 hidden">
          <a href="/#about"
            ><button class="font-bold focus:outline-none">ABOUT</button></a
          >
          <a href="/#portfolio"
            ><button class="font-bold focus:outline-none">PORTFOLIO</button></a
          >
          <a href="/#contact"
            ><button class="font-bold focus:outline-none">CONTACT</button></a
          >
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
          <a href="/"><i class="far fa-times"></i></a>
        </div>

        <div
          class="bg-white text-black w-4/5 h-screen z-20 fixed right-2 top-2 text-xl pt-8"
        >
          <!--  -->
          <div class="pl-6">
            <a href="/#portfolio"
              ><button
                @click="mobileMenu = false"
                class="block font-bold focus:outline-none"
              >
                PORTFOLIO
              </button></a
            >
            <a href="/#contact"
              ><button
                @click="mobileMenu = false"
                class="block font-bold focus:outline-none my-12"
              >
                CONTACT
              </button></a
            >
            <a href="/#about"
              ><button
                @click="mobileMenu = false"
                class="block font-bold focus:outline-none"
              >
                ABOUT
              </button></a
            >
          </div>
        </div>
      </div>
      <!-- Navbar ends -->
      <div>
        <div class="mt-6 xl:mt-12">
          <!--  -->
          <div class="items-center lg:flex">
            <div class="">
              <img
                class="lg:rounded-full inset-0 object-cover lg:ml-44 ml-0 w-full h-96 bg-cover"
                src="./assets/portfolio-img2.jpg"
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
                class="xl:text-7xl lg:text-6xl md:text-6xl sm:text-5xl text-5xl py-5 font-bold xl:block flex justify-center md:hidden"
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
        <a href="/#bottom"
          ><i class="text-gray-300 fal fa-arrow-down text-4xl animate-bounce"></i
        ></a>
      </div>
    </section>

    <!-- About Me -->
    <section
      id="about"
      class="pb-7 min-h-screen w-full lg:px-24 md:px-12 px-4 pt-7"
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
    <!-- Portfolio -->
    <section
      id="portfolio"
      class="pb-7 min-h-screen w-full lg:px-24 md:px-12 px-4 pt-7"
      style="background-color: #222222"
    >
      <div class="uppercase text-white text-3xl font-semibold text-center">
        my portfolio
      </div>

      <div class="grid grid-cols-2 gap-16 mt-7 mx-8">
        <div
          v-for="portfolio in portfolios"
          :key="portfolio.index"
          class="h-72 relative overflow-hidden"
        >
          <img
            :src="require(`./assets/${portfolio.image}`)"
            :alt="portfolio.title"
            class="w-full h-full inset-0 object-cover rounded-md z-0 absolute overflow-hidden"
          />
          <div
            class="bg-blue-500 bg-opacity-50 z-10 w-full h-full absolute p-8 opacity-0 hover:opacity-100 duration-1000 rounded-md"
          >
            <div
              class="text-center text-white border-2 border-gray-200 w-full h-full rounded-md p-2 z-20 relative"
            >
              <p class="text-2xl font-semibold">{{ portfolio.title }}</p>

              <p class="text-xl">{{ portfolio.description }}</p>
              <a :href="portfolio.link" class="absolute bottom-2 -ml-14 pl-0.5">
                <button class="bg-black px-3 py-2 rounded-md cursor-pointer">
                  Click Here
                </button>
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Contact Me -->
    <section
      id="contact"
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
      <div id="bottom" class="flex justify-center">
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
      portfolios: [
        {
          image: "port1.jpg",
          title: "Invoice App",
          description:
            "An app that gives invoice details with payment status and printing options!",
          link: "https://invoice-web.netlify.app/",
        },
        {
          image: "port2.jpg",
          title: "Room Booking App",
          description:
            "An app that allows you select your room of choice, depending on size and other preferences!",
          link: "https://luxurious-rooms.netlify.app/",
        },
        {
          image: "port3.jpg",
          title: "Question and Answer App",
          description:
            "A web based game that allows audiences to answer questions and review their performance at the end of the game!",
            link: "https://q-a.netlify.app/",
        },
        {
          image: "port4.jpg",
          title: "Flight RealTime Info App",
          description: "An app that shows near-realtime information of all flights around the world!",
          link: "https://opensky-coven-works.netlify.app/",
        },
        {
          image: "port5.jpg",
          title: "Invoice App",
          description: "An invoice app that do, do and do, that do!",
        },
        {
          image: "port4.jpg",
          title: "Invoice App",
          description: "An invoice app that do, do and do, that do!",
        },
      ],
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
          icon: "fal fa-code text-base",
          progress: "95%",
        },
        {
          name: "Bootstrap",
          icon: "fab fa-bootstrap text-purple-400",
          progress: "90%",
        },
        {
          name: "Material UI",
          icon: "fal fa-code text-base",
          progress: "70%",
        },
      ],
    };
  },
};
</script>

<style></style>
