<template>
  <div>
    <div class="nav-drawer" :class="{'nav-drawer__close': !drawer, 'nav-drawer__open': drawer}">
      <div v-if="title" class="nav-drawer__header">
        <div class="row p-2">
          <div class="col-9">
            <span class="nav-drawer__header__title">{{ title }}</span>
          </div>
          <div class="col-3" style="cursor: pointer" @click="drawer = false">
            <i class="fas fa-chevron-left" />
          </div>
        </div>
      </div>
      <slot />
    </div>
    <div
      v-show="drawer"
      class="nav-close"
      :class="{'nav-close__active': drawer}"
      @click="drawer = false"
    />
  </div>
</template>
<script>
export default {
  name: "NavDrawer",
  props: {
    value: {
      type: Boolean,
      required: true,
    },
    title: {
      type: String,
      default: "",
    },
  },
  computed: {
    drawer: {
      get() {
        return this.value;
      },
      set(value) {
        this.$emit("input", value);
      },
    },
  },
};
</script>

<style lang="scss" scoped>
.nav-drawer {
  overflow: auto;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 9999;
  width: 90%;
  max-width: 200px;
  height: 100%;
  &__close {
    transition: 0.3s ease-in-out;
    -webkit-transform: translateX(-105%);
    transform: translateX(-105%);
  }
  &__open {
    transition: 0.3s ease-in-out;
    -webkit-transform: translateX(0%);
    transform: translateX(0%);
    box-shadow: 6px 0 25px rgba(0, 0, 0, 0.15);
  }
  &__header {
    border-bottom: 3px double;
    &__title {
      font-weight: bold;
    }
  }
  &__item {
    padding: 0.5rem;
    border-bottom: 1px solid;
    &:hover {
      cursor: pointer;
      transition: 0.3s;
    }
  }
  background-color: white;
}

.nav-close {
  position: fixed;
  z-index: 99;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: black;
  opacity: 0.5;
  transition: 0.3s ease-in-out;
  cursor: pointer;
}
</style>