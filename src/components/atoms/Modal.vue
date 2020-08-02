<template>
  <div class="card">
    <button class @click="showModal = !showModal">開くボタン</button>
    <transition>
      <div class v-if="showModal">
        <div class>
          <p>ひらいたよ</p>
          <button @click="click">とじる</button>
        </div>
      </div>
    </transition>
  </div>
</template>
<script>
export default {
    data() {
        return {
            showModal: false
        }
    },
    methods: {
        click() {
            this.showModal = false;
        }
    }
};
</script>
<style scoped>
</style>