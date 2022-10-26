<template>
  <div>
    <main class="mt-20">
      <div class="container mx-auto px-4">
        <div class="w-full flex justify-center">
          <div class="text-center w-full md:w-[60%]">
            <h3 class="text-2xl lg:text-4xl font-semibold mb-6">
              Create New CV
            </h3>
            <p class="text-lg mb-6">Copy an existing resume</p>
            <div class="lg:flex w-full md:space-x-2">
              <div
                class="shadow-lg p-3 rounded-lg w-full lg:w-[75%] flex mb-4 lg:mb-0"
              >
                <select
                  name=""
                  id=""
                  class="w-full border-none outline-none text-lg text-gray-600"
                >
                  <option value="">My Website 2020-10-26</option>
                  <option value="">My Website 2020-10-26</option>
                  <option value="">My Website 2020-10-26</option>
                </select>
              </div>
              <div
                class="w-full lg:w-[15%] md:flex py-3 lg:py-0 justify-center bg-blue-400 rounded-lg text-white text-lg font-semibold hover:bg-blue-500 transition duration-300"
              >
                <button>Copy</button>
              </div>
            </div>
            <p class="text-lg mt-6">Or choose from one of the options below</p>
          </div>
        </div>
        <section class="mt-16 flex justify-center">
          <div class="bg-gray-100 rounded-xl p-4 lg-[90%] xl:w-[80%]">
            <div
              class="grid md:grid-cols-2 lg:grid-cols-3 gap-4 auto-rows-[minmax(320px)]"
            >
              <!-- =======Card 1================== -->
              <a
                href="#"
                class="bg-gray-400 rounded-xl flex h-full justify-center items-center group hover:bg-gray-600 transition-all duration-500"
              >
                <div>
                  <div class="flex justify-center items-center">
                    <img
                      src="../assets/img/document-good.svg"
                      alt=""
                      class=""
                    />
                  </div>
                  <p class="font-semibold text-xl mt-2 text-center text-white">
                    Use existing resume
                  </p>

                  <div class="px-8">
                    <p class="text-center text-white">
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Ut maiores corporis natus inventore neque
                    </p>
                  </div>
                </div>
              </a>
              <!-- =====End==Card 1================== -->
              <!-- =======Card 2================== -->
              <a
                href="#"
                class="bg-gray-400 rounded-xl flex justify-center items-center group hover:bg-gray-600 transition-all duration-500"
              >
                <div>
                  <div class="flex justify-center">
                    <img
                      src="../assets/img/document-good.svg"
                      alt=""
                      class=""
                    />
                  </div>
                  <p class="font-semibold text-xl mt-2 text-center text-white">
                    Use sample content
                  </p>

                  <div class="px-8">
                    <p class="text-center text-white">
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Ut maiores corporis natus inventore neque v
                    </p>
                  </div>
                </div>
              </a>
              <!-- =====End==Card 2================== -->
              <!-- =======Card 2================== -->
              <a
                href="#"
                class="bg-gray-400 rounded-xl flex justify-center items-center group hover:bg-gray-600 transition-all duration-500"
              >
                <div>
                  <div class="flex justify-center">
                    <img
                      src="../assets/img/document-good.svg"
                      alt=""
                      class=""
                    />
                  </div>
                  <p class="font-semibold text-xl mt-2 text-center text-white">
                    Use sample content
                  </p>

                  <div class="px-8">
                    <p class="text-center text-white">
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Ut maiores corporis natus inventore neque v
                    </p>
                  </div>
                </div>
              </a>
              <!-- =====End==Card 2================== -->
            </div>
          </div>
        </section>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: "createnew",
};
</script>

<style></style>
