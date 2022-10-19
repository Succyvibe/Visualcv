<template>
  <div
    class="absolute top-[50%] left-[50%] translate-x-[-50%] translate-y-[-50%] w-[40%] h-[40rem] bg-white rounded-md shadow-lg z-30 hidden"
  >
    <div class="bg-blue-50 h-[70%] p-6">
      <button
        class="absolute top-[1.2rem] right-[2rem] text-5xl text-gray-600 border-0 bg-none"
      >
        &times;
      </button>
      <div class="p-10">
        <h1 class="text-3xl text-center">You've hit your resume limit</h1>
      </div>
      <div
        class="absolute top-[50%] left-[50%] translate-x-[-50%] translate-y-[-50%]"
      >
        <img src="../assets/img/upgrade_resume.png" alt="" />
      </div>
    </div>
    <div class="p-10">
      <div class="text-center">
        <small class="text-lg">
          To create unlimited resumes, websites, and cover letters please
          upgrade to VisualCV Pro.</small
        >
      </div>

      <div class="w-full grid grid-cols-2 flex-1 gap-3 mt-6">
        <a
          href="#"
          class="border border-blue-200 text-blue-200 hover:bg-blue-200 transition duration-500 rounded-lg flex justify-center items-center font-medium"
          >Not Yet</a
        >
        <a
          href="#"
          class="bg-blue-500 text-white px-4 py-2 flex justify-center items-center font-medium rounded-lg"
          >Upgrade</a
        >
      </div>
    </div>
  </div>
  <div class="overlay absolute top-0 left-0 h-full hidden w-full"></div>
</template>

<script>
export default {
  name: "Modal",
};
</script>

<style scoped>
.show-modal {
  font-size: 2rem;
  font-weight: 600;
  padding: 1.75rem 3.5rem;
  margin: 5rem 2rem;
  border: none;
  background-color: #fff;
  color: #444;
  border-radius: 10rem;
  cursor: pointer;
}

.close-modal {
  position: absolute;
  top: 1.2rem;
  right: 2rem;
  font-size: 5rem;
  color: #333;
  cursor: pointer;
  border: none;
  background: none;
}

/* -------------------------- */
/* CLASSES TO MAKE MODAL WORK */
.hidden {
  display: none;
}

.modal {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);

  background-color: white;
  padding: 6rem;
  border-radius: 5px;
  box-shadow: 0 3rem 5rem rgba(0, 0, 0, 0.3);
  z-index: 10;
}

.overlay {
  background-color: rgba(0, 0, 0, 0.6);
  backdrop-filter: blur(3px);
  z-index: 1;
}
</style>
