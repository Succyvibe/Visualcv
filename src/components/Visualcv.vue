<template>
  <main class="mt-20">
    <div class="container mx-auto px-4">
      <h1 class="text-2xl md:text-3xl font-semibold">
        Hey Success, Welcome to VisualCv!
      </h1>
      <p class="text-md md:text-xl">
        You're on your way to landing your dream job
      </p>

      <!-- --===============CARD SECTION=========== -->
      <section class="mt-6">
        <div class="card-wrapper">
          <div
            class="bg-gray-100 md:grid md:grid-cols-2 lg:grid-cols-2 xl:grid-cols-4 hidden gap-5 flex-1 p-5 rounded-xl mb-5"
          >
            <a href="#">
              <div
                class="bg-gray-300 shadow-md rounded-xl flex space-x-3 h-full items-center px-4 py-2"
              >
                <div class="">
                  <img
                    class="w-16"
                    src="../assets/img/document-good.svg"
                    alt=""
                  />
                </div>
                <div>
                  <p class="text-gray-500 font-bold text-sm">Create a Resume</p>
                  <p class="text-gray-500 text-sm">Land your next job</p>
                </div>
              </div>
            </a>
            <a href="#" class="">
              <div
                class="bg-white flex-grow shadow-lg shadow-bg-blue-200 rounded-xl flex space-x-3 px-4 py-2 items-center hover:shadow-lg hover:shadow-blue-100"
              >
                <div>
                  <img class="w-20" src="../assets/img/document-2.svg" alt="" />
                </div>
                <div>
                  <p class="text-gray-500 font-bold text-sm">
                    Create a Website
                  </p>
                  <p class="text-gray-500 text-sm">Market yourself</p>
                </div>
              </div>
            </a>
            <a href="#">
              <div
                class="bg-white flex-grow shadow-bg-blue-500 rounded-xl flex space-x-3 px-4 py-2 items-center hover:shadow-lg hover:shadow-blue-100"
              >
                <div>
                  <img class="w-20" src="../assets/img/document-3.svg" alt="" />
                </div>
                <div>
                  <p class="text-gray-500 font-bold text-sm">
                    Create a Journal Entry
                  </p>
                  <p class="text-gray-500 text-sm">Track career heights</p>
                </div>
              </div>
            </a>
            <a href="#">
              <div
                class="bg-gray-300 flex-grow shadow-lg shadow-bg-blue-200 rounded-xl flex space-x-3 px-4 py-2 h-full items-center hover:shadow-lg hover:shadow-blue-100"
              >
                <div>
                  <img class="w-16" src="../assets/img/document-4.svg" alt="" />
                </div>
                <div>
                  <p class="text-gray-500 font-bold text-sm">
                    Create a Cover letter
                  </p>
                  <p class="text-gray-500 text-sm">Show your personality</p>
                </div>
              </div>
            </a>
          </div>
          <!-- --===================sm display==================== -->
          <div class="md:hidden bg-white shadow-md rounded-xl mb-4">
            <div
              class="flex justify-between p-5 cursor-pointer transition duration-700"
              id="dropdown-btn"
              @click="toggleDiv"
            >
              <h5 class="font-semibold">Get The Best From VisualCV</h5>
              <button class="w-4">
                <img src="../assets/img/Vector.png" alt="" class="w-full" />
              </button>
            </div>
            <Transition>
              <div class="hidde" v-if="isVisible">
                <a href="#">
                  <div
                    class="flex justify-between bg-white shadow-md p-5 border-b-2"
                  >
                    <div class="flex space-x-3">
                      <div>
                        <img src="../assets/img/check.png" alt="" />
                      </div>
                      <h5 class="font-semibold">Create a Resume</h5>
                    </div>
                    <div>
                      <img src="../assets/img/add-icon.png" class="" alt="" />
                    </div>
                  </div>
                </a>

                <!-- ----------Create a website------------ -->
                <a href="#">
                  <div
                    class="flex justify-between bg-white shadow-md p-5 border-b-2"
                  >
                    <div class="flex space-x-3">
                      <div>
                        <img src="../assets/img/check.png" alt="" />
                      </div>
                      <h5 class="font-semibold">Create a Website</h5>
                    </div>
                    <div>
                      <img src="../assets/img/add-icon.png" alt="" />
                    </div>
                  </div>
                </a>
                <!-- ============Create a Journal===================== -->
                <a href="#">
                  <div
                    class="flex justify-between bg-white shadow-md p-5 border-b-2"
                  >
                    <div class="flex space-x-3">
                      <div>
                        <img src="../assets/img/check.png" alt="" />
                      </div>
                      <h5 class="font-semibold">Create a Website</h5>
                    </div>
                    <div>
                      <img src="../assets/img/add-icon.png" alt="" />
                    </div>
                  </div>
                </a>

                <!-- ===========Create over Letter======================= -->
                <a href="#">
                  <div class="flex justify-between bg-white shadow-md p-5">
                    <div class="flex space-x-3">
                      <div>
                        <img src="../assets/img/check.png" alt="" />
                      </div>
                      <h5 class="font-semibold">Create a Website</h5>
                    </div>
                    <div>
                      <img src="../assets/img/add-icon.png" alt="" />
                    </div>
                  </div>
                </a>
              </div>
            </Transition>
          </div>
          <!-- ------------------End sm display -->

          <!-- =====Grid wrapper========================== -->
          <div class="grid xl:grid-cols-2 gap-4 grid-rows-3 mb-5">
            <!-- =================Grid-card-1================= -->
            <div class="bg-red-100 p-4 rounded-xl row-span-3">
              <!-- -top card---------------- -->
              <div class="flex justify-between mb-4">
                <div>
                  <div class="flex items-center space-x-3">
                    <img src="../assets/img/document-text.png" alt="" />
                    <a href="#" class="text-lg font-semibold">Resumes</a>
                  </div>
                </div>
                <button
                  class="bg-white text-sm font-semibold text-blue-400 px-3 rounded-md hover:bg-blue-200 transition duration-75"
                >
                  See All
                </button>
              </div>
              <!-- -------end top card------------------- -->

              <!-- ==============Inner grid card============================= -->
              <div
                class="grid md:grid-cols-3 xl:grid-cols-2 gap-4 auto-rows-[320px] flex-1"
              >
                <!-- =======Card 1================== -->
                <a
                  href="#"
                  class="bg-orange-200 rounded-xl flex justify-center items-center group hover:bg-orange-300 transition-all duration-500"
                  @click="onClick()"
                >
                  <div>
                    <div class="flex justify-center">
                      <img
                        src="../assets/img/add-icon.png"
                        alt=""
                        class="group-hover:shadow-lg w-[40px]"
                      />
                    </div>
                    <p class="font-semibold">Create New</p>
                  </div>
                </a>

                <!-- =====End==Card 1================== -->
                <!-- =======Card 2================== -->
                <a
                  href="#"
                  class="bg-orange-200 hover:bg-orange-300 duration-500 transition rounded-xl flex justify-center items-center relative card-banner"
                >
                  <img
                    src="../assets/img/cover-letter-img.jpg"
                    class="w-full h-full rounded-xl"
                    alt=""
                  />
                  <div
                    class="absolute top-[2px] left-[10px] bg-blue-700 text-white rounded-lg px-2 mt-8 font-semibold"
                  >
                    Pro
                  </div>
                  <div
                    class="absolute h-full w-full top-0 left-0 border-t-2 transition"
                  >
                    <div
                      class="w-full transition-all absolute bottom-0 bg-white px-4 border-t-2"
                    >
                      <div class="w-full flex justify-between items-center">
                        <div>
                          <div class="hover:bottom-[46% z-20]">
                            <h4 class="font-semibold">My VisualCV</h4>
                            <p>Updated-Oct 12</p>
                          </div>
                        </div>
                        <div class="flex items-center">
                          <img src="../assets/img/check.png" alt="" />
                        </div>
                      </div>
                    </div>
                    <div class="card-action-list">
                      <img src="../assets/img/add-icon.png" alt="" />
                      <img src="../assets/img/add-icon.png" alt="" />
                      <img src="../assets/img/add-icon.png" alt="" />
                    </div>
                  </div>
                </a>
                <!-- =====End==Card 2================== -->
                <!-- =======Card 3================== -->
                <a
                  href="#"
                  class="bg-orange-200 hover:bg-orange-300 duration-500 transition rounded-xl flex justify-center items-center"
                >
                  <div>
                    <div class="flex justify-center">
                      <img src="../assets/img/add-icon.png" alt="" />
                    </div>
                    <p class="font-semibold">Create New</p>
                  </div>
                </a>
                <!-- =====End==Card 3================== -->
                <!-- =======Card 4================== -->
                <a
                  href="#"
                  class="bg-orange-200 hover:bg-orange-300 duration-500 transition rounded-xl flex justify-center items-center md:hidden xl:flex"
                >
                  <div>
                    <div class="flex justify-center">
                      <img src="../assets/img/add-icon.png" alt="" />
                    </div>
                    <p class="font-semibold">Create New</p>
                  </div>
                </a>
                <!-- =====End==Card 4================== -->
              </div>
            </div>

            <!-- =============Grid card-2===================== -->
            <div class="row-span-3 md:px-4">
              <div class="grid grid-rows-2 gap-4 h-full">
                <div class="bg-blue-100 rounded-xl p-4">
                  <div class="flex items-center space-x-3">
                    <img src="../assets/img/document-text.png" alt="" />
                    <a href="#" class="text-lg font-semibold">Websites</a>
                  </div>

                  <a href="#">
                    <div
                      class="bg-blue-200 rounded-xl mt-5 h-[80%] flex justify-center items-center website hover:bg-blue-300 p-12"
                    >
                      <div
                        class="flex flex-col justify-center items-center h-full w-full"
                      >
                        <div class="w-32 h-32 flex relative">
                          <img
                            class="w-full h-full cover"
                            src="../assets/img/document-text.png"
                            alt=""
                          />
                          <img
                            src="../assets/img/add-icon.png"
                            class="absolute top-[50%] left-[50%] translate-x-[-50%] translate-y-[-50%] child w-12"
                            alt=""
                          />
                        </div>
                        <p class="text-center font-semibold text-xl my-3">
                          Website
                        </p>
                        <p class="text-gray-500 text-center text-sm">
                          Build a personal/professional portfolio to showcase
                          your skills online
                        </p>
                      </div>
                    </div>
                  </a>
                </div>
                <div class="bg-gray-100 rounded-xl p-4">
                  <div class="flex items-center space-x-3">
                    <img src="../assets/img/document-text.png" alt="" />
                    <a href="#" class="text-lg font-semibold">Websites</a>
                  </div>

                  <a href="#">
                    <div
                      class="bg-lime-100 rounded-xl mt-5 h-[80%] flex justify-center items-center hover:bg-lime-200"
                    >
                      <div
                        class="flex flex-col justify-center items-center h-full w-full website"
                      >
                        <div class="w-32 h-32 flex relative">
                          <img
                            class="w-full h-full cover"
                            src="../assets/img/document-text.png"
                            alt=""
                          />

                          <img
                            src="../assets/img/add-icon.png"
                            class="absolute top-[50%] left-[50%] translate-x-[-50%] translate-y-[-50%] child w-12"
                            alt=""
                          />
                        </div>
                        <p class="text-center font-semibold text-xl my-3">
                          Website
                        </p>
                        <p class="text-gray-500 text-center text-sm">
                          Build a personal/professional portfolio to showcase
                          your skills online
                        </p>
                      </div>
                    </div>
                  </a>
                </div>
              </div>
            </div>
          </div>

          <!-- -------------Ed of grid wrapper------------------- -->
        </div>
      </section>
      <!-- --============END===CARD SECTION=========== -->

      <section class="my-4">
        <div
          class="grid xl:grid-cols-2 flex-1 auto-rows-[minmax(320px,_2fr)] xl:space-x-4 gap-4"
        >
          <div class="bg-gray-200 rounded-xl p-4">
            <div class="flex space-x-3">
              <img src="../assets/img/document-text.png" alt="" />
              <a href="#" class="text-lg font-semibold">VisualCV Expert</a>
            </div>
            <div
              class="space-x-9 md:items-center h-full md:flex-row flex flex-col-reverse"
            >
              <div class="md:w-[40%] my-10">
                <img
                  src="../assets/img/expert-free-user.png"
                  class="w-full h-full cover"
                  alt=""
                />
              </div>
              <div class="md:w-[60%]">
                <h2
                  class="text-2xl text-center md:text-start md:text-3xl font-semibold mb-4"
                >
                  Professional Resume/CV Writing & Reviews
                </h2>
                <p
                  class="text-gray-600 font-medium mb-6 text-center md:text-start"
                >
                  Get your resume professionally written by our resume experts,
                  or get a 10-minute video review of your current resume!
                </p>
                <a href="#" class="text-blue-500 font-medium text-center"
                  >Improve my resume now</a
                >
              </div>
            </div>
          </div>
          <div class="bg-gray-100 rounded-xl p-4">
            <div class="flex justify-between mb-4">
              <div>
                <div class="flex items-center space-x-3">
                  <img src="../assets/img/document-text.png" alt="" />
                  <a href="#" class="text-lg font-semibold">Resumes</a>
                </div>
              </div>
              <button
                class="bg-white text-sm font-semibold text-blue-400 px-3 rounded-md hover:bg-blue-200 transition duration-75"
              >
                See All
              </button>
            </div>

            <div class="grid md:grid-cols-2 gap-4 auto-rows-[320px]">
              <!-- =======Card 1================== -->
              <a
                href="#"
                class="bg-orange-200 rounded-xl flex justify-center items-center group hover:bg-orange-300 transition-all duration-500"
              >
                <div>
                  <div class="flex justify-center">
                    <img
                      src="../assets/img/add-icon.png"
                      alt=""
                      class="group-hover:shadow-lg w-[40px]"
                    />
                  </div>
                  <p class="font-semibold">Create New</p>
                </div>
              </a>
              <!-- =====End==Card 1================== -->
              <!-- =======Card 2================== -->
              <a
                href="#"
                class="bg-orange-200 hover:bg-orange-300 duration-500 transition rounded-xl flex justify-center items-center relative card-banner"
              >
                <img
                  src="../assets/img/cover-letter-img.jpg"
                  class="w-full h-full rounded-xl"
                  alt=""
                />
                <div
                  class="absolute top-[2px] left-[10px] bg-blue-700 text-white rounded-lg px-2 mt-8 font-semibold"
                >
                  Pro
                </div>
                <div
                  class="absolute h-full w-full top-0 left-0 border-t-2 transition"
                >
                  <div
                    class="w-full transition-all absolute bottom-0 bg-white px-4 border-t-2"
                  >
                    <div class="w-full flex justify-between items-center">
                      <div>
                        <div class="hover:bottom-[46% z-20]">
                          <h4 class="font-semibold">My VisualCV</h4>
                          <p>Updated-Oct 12</p>
                        </div>
                      </div>
                      <div class="flex items-center">
                        <img src="../assets/img/check.png" alt="" />
                      </div>
                    </div>
                  </div>
                  <div class="card-action-list">
                    <img src="../assets/img/add-icon.png" alt="" />
                    <img src="../assets/img/add-icon.png" alt="" />
                    <img src="../assets/img/add-icon.png" alt="" />
                  </div>
                </div>
              </a>
              <!-- =====End==Card 2================== -->
            </div>
          </div>
        </div>

        <div class="bg-gray-100 mt-5 p-4 rounded-xl">
          <div class="flex justify-between items-center">
            <div class="flex items-center space-x-3">
              <img src="../assets/img/document-text.png" alt="" />
              <a href="#" class="text-lg font-semibold">Websites</a>
            </div>
            <a
              href="#"
              class="bg-white px-5 py-2 text-blue-500 text-sm font-medium rounded-lg"
              >Go to knowledge center</a
            >
          </div>
          <h2 class="text-3xl font-semibold my-4">
            Need some help getting started?
          </h2>

          <ul
            class="flex py-[25px] list-none overflow-x-scroll snap-x-mandatory"
          >
            <li class="cardd relative">
              <img
                src="../assets/img/enterprise_hero_img3_(1).png"
                class="w-full h-full hover:scale-125 transition duration-500"
                alt=""
              />
              <div class="absolute bottom-10 left-4">
                <div class="w-full py-3 bg-white px-10 rounded">
                  <h3 class="font-semibold text-md">
                    Cover Letter example guide
                  </h3>
                  <a href="#" class="text-blue-300">Read Post</a>
                </div>
              </div>
            </li>
            <li class="cardd relative">
              <img
                src="../assets/img/enterprise_hero_img3_(2).png"
                class="w-full h-full hover:scale-125 transition duration-500"
                alt=""
              />
              <div class="absolute bottom-10 left-4">
                <div class="w-full py-3 bg-white px-10 rounded">
                  <h3 class="font-semibold text-md">
                    How to Write a Reusme in 2022
                  </h3>
                  <a href="#" class="text-blue-300">Read post</a>
                </div>
              </div>
            </li>
            <li class="cardd relative">
              <img
                src="../assets/img/enterprise_hero_img3_(1).png"
                class="w-full h-full hover:scale-125 transition duration-500"
                alt=""
              />

              <div class="absolute bottom-10 left-4 px-4 bg-white rounded">
                <h3 class="font-semibold text-md">
                  Online Career Resources Guide
                </h3>
                <a href="#" class="text-blue-300">Read more</a>
              </div>
            </li>
            <li class="cardd relative">
              <img
                src="../assets/img/enterprise-hero-img.png"
                class="w-full h-full hover:scale-125 transition duration-500"
                alt=""
              />
              <div class="absolute bottom-10 left-4 px-4 bg-white rounded">
                <h3 class="font-semibold text-md">2022 Hiring Statistics</h3>
                <a href="#" class="text-blue-300">Read Post</a>
              </div>
            </li>
            <li class="cardd relative">
              <img
                src="../assets/img/enterprise-hero-img.png"
                class="w-full h-full hover:scale-125 transition duration-500"
                alt=""
              />
              <div class="absolute bottom-10 left-4 px-4 bg-white rounded">
                <h3 class="font-semibold text-md">2022 Hiring Statistics</h3>
                <a href="#" class="text-blue-300">Read Post</a>
              </div>
            </li>
            <li class="cardd relative">
              <img
                src="../assets/img/enterprise-hero-img.png"
                class="w-full h-full hover:scale-125 transition duration-500"
                alt=""
              />
              <div class="absolute bottom-10 left-4 px-4 bg-white rounded">
                <h3 class="font-semibold text-xl">2022 Hiring Statistics</h3>
                <a href="#" class="text-blue-300">Read Post</a>
              </div>
            </li>
          </ul>

          <div class="flex justify-between items-center mt-5">
            <i class="fa fa-backward"></i>
            <i class="fa fa-forward"></i>
          </div>
        </div>
      </section>
    </div>
  </main>
</template>

<script>
export default {
  name: "Visualcv",
  data() {
    return {
      isVisible: false,
    };
  },
  methods: {
    toggleDiv() {
      this.isVisible = !this.isVisible;
    },
  },
  onClick() {
    this.$emit("toogle-modal");
  },
};
</script>

<style scoped>
.v-enter-active,
.v-leave-active {
  transition: opacity 0.5s ease;
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
}
</style>
