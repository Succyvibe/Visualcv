<template>
  <div class="home">
    <Visualcv />
    <Modal @toggle-modal="toggleModal" />
    <SeeAll />
  </div>
</template>

<script>
// @ is an alias to /src
import Visualcv from "@/components/Visualcv.vue";
import Modal from "@/components/Modal.vue";
import SeeAll from "@/components/SeeAll.vue";

export default {
  name: "HomeView",
  components: {
    Visualcv,
    Modal,
    SeeAll,
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
