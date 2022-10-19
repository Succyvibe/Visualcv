<template>
  <div class="home">
    <Visualcv />
    <Modal @toggle-modal="toggleModal" />
  </div>
</template>

<script>
// @ is an alias to /src
import Visualcv from "@/components/Visualcv.vue";
import Modal from "@/components/Modal.vue";

export default {
  name: "HomeView",
  components: {
    Visualcv,
    Modal,
  },
  data() {
    return {
      showModal: false,
    };
  },
  methods: {
    toggleModal() {
      this.showModal = true;
    },
  },
};
</script>
