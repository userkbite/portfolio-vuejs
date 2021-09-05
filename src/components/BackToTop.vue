<template>
  <a id="back-to-top" @click="backToTop()" v-if="showButton">
    <span class="material-icons"> 🚀 </span>
  </a>
</template>

<script>
export default {
  name: "BackToTop",
  data() {
    return {
      showButton: false,
    };
  },
  mounted() {
    window.addEventListener("scroll", this.onScroll);
  },
  beforeDestroy() {
    window.removeEventListener("scroll", this.onScroll);
  },
  methods: {
    onScroll() {
      this.windowTop = window.top.scrollY;
      this.showButton = this.windowTop > 600;
    },
    backToTop() {
      document.body.scrollTop = 0; // For Safari
      document.documentElement.scrollTop = 0; // For Chrome, Firefox, IE and Opera
    },
  },
};
</script>

<style lang="scss">
#back-to-top {
  $white: #ffffff;
  $black: #1f1f1f;
  cursor: pointer;
  position: fixed;
  bottom: 1rem;
  right: 1rem;
  padding: 1.1rem 1.2rem;
  background-color: $black;
  color: $white;
  border-radius: 0.5rem;
  text-decoration: none;
  z-index: 99;
  -webkit-tap-highlight-color: transparent;
  &:hover {
    background-color: $white;
    color: $white;
    transform: scale(105%);
  }
}
</style>