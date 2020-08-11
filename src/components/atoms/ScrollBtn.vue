<template>
  <transition name="fade">
    <div id="pagetop" class="fixed right-0 bottom-0 cursor"  v-show="scrollY > 100" @click="moveToTop">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="48"
        height="48"
        viewBox="0 0 24 24"
        fill="none"
        stroke="#4a5568"
        stroke-width="1"
        stroke-linecap="square"
        stroke-linejoin="arcs"
      >
        <path d="M18 15l-6-6-6 6" />
      </svg>
    </div>
  </transition>
</template>

<script>
export default {
  name: "ScrollBtn",
  data() {
    return {
      scrollTimer: 0,
      scrollY: 0,
    };
  },
  mounted() {
    addEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      if (this.scrollTimer) {
        return this;
      }
      this.scTrollimer = setTimeout(() => {
        this.scrollY = scrollY;
        clearTimeout(this.scrollTimer);
        this.scTimer = 0;
      }, 100);
    },
    moveToTop() {
      scrollTo({
        top: 0,
        behavior: "smooth",
      });
    },
  },
};
</script>
<style scoped>
.cursor {
  cursor: pointer;
}
</style>