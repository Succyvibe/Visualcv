<template>
  <div class="container mx-auto px-4">
    <div class="md:flex justify-between items-center my-8">
      <div>
        <h1 class="text-2xl font-semibold">Resume</h1>
        <p>Create custom resumes for each application</p>
      </div>
      <button
        class="bg-blue-400 px-3 py-2 text-white hover:shadow-lg hover:shadow-blue-400 transition duration-500 space-x-3 rounded-md"
      >
        <span><i class="fa fa-plus"></i></span>
        <span>Create New</span>
      </button>
    </div>

    <section class="mb-20">
      <!-- ============CARDS==================== -->
      <div class="">
        <div class="bg-red-100 min-h-[360px] rounded-2xl relative p-4 mb-5">
          <div>
            <span>
              <i class="fa fa-pin"></i>
            </span>
            <span class="font-medium">Pinned Resumes</span>
          </div>

          <div
            class="absolute top-[50%] left-[50%] translate-x-[-50%] translate-y-[-50%]"
          >
            <img src="../assets/img/document-2.svg" alt="" />
            <div class="text-center">
              <p class="text-xl font-medium mt-0">No Resumes Pinned</p>
              <small class="font-medium text-sm"
                >Pin resumes to find them more easily!</small
              >
            </div>
          </div>
        </div>
        <div
          class="md:flex justify-between h-[300px] md:h-[100px] mt-10 bg-blue-100"
        >
          <div class="w-full md:w-[30%] xl:w-[20%] h-[30%] md:h-full">
            <img
              src="../assets/img/enterprise_hero_img3_(1).png"
              alt=""
              class="w-full h-full cover"
            />
          </div>
          <div
            class="w-full md:w-[50%] xl:w-[60%] md:h-full px-5 xl:pt-8 md:pt-0 pt-8"
          >
            <div class="flex xl:ustify-center xl:items-center h-full">
              <div class="flex flex-col xl:justify-center h-ful">
                <h3 class="text-xl xl:text-2xl font-semibold">
                  Your dream job is waiting
                </h3>
                <p class="text-md xl:text-lg font-medium text-gray-600">
                  VisualCV Pro resume templates are proven to land more
                  interviews.
                </p>
              </div>
            </div>
          </div>

          <div class="flex items-center w-full md:w-[30%] px-5 pt-8 md:pt-0">
            <button class="bg-blue-400 px-3 py-2 rounded-lg text-white w-full">
              Upgrade Now
            </button>
          </div>
        </div>

        <div class="bg-gray-100 mt-5 p-4 rounded-xl">
          <div class="flex justify-between items-center">
            <div class="flex items-center space-x-2">
              <img src="../assets/img/document-text.png" alt="" />
              <a href="#" class="text-lg font-semibold">All Resume</a>
            </div>
          </div>

          <ul
            class="flex py-[25px] list-none overflow-x-scroll snap-x-mandatory"
          >
            <li class="cardd relative">
              <a
                href="#"
                class="bg-blue-200 rounded-xl flex justify-center items-center group hover:bg-blue-300 transition-all duration-500 h-full"
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
            </li>
            <li class="cardd relative">
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
            </li>
          </ul>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "SeeAll",
};
</script>

<style></style>
