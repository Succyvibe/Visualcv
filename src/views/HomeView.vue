<template>
  <div class="home">
    <createnew />
    <Portfolio />
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
import Portfolio from "@/components/Portfolio.vue";
import createnew from "@/components/createnew.vue";

export default {
  name: "HomeView",
  components: {
    Visualcv,
    Modal,
    SeeAll,
    Portfolio,
    createnew,
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
