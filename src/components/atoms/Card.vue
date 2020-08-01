<template>
  <div class="profile-item card text-center" ontouchstart @click="reverse()">
      <div v-if="!is_reversed">
          <div class="prifile-title card-header">
              {{ title }}
          </div>
          <div class="profile-body card-body p-2">
              <img :src="dumpImg()" style="height: 180px">
          </div>
      </div>

    <div v-else>
        <div class="profile-title card-header text-info">
            {{ title}}
        </div>
        <div class="profile-body card-body p-2">
            {{ comment }}
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        title: String,
        logo: String,
        comment: String
    },
    data() {
        return {
            is_reversed: false
        }
    },
    methods: {
        reverse() {
            this.is_reversed = !this.is_reversed;
        },
        dumpImg() {
            return this.logo;
        }
    }
}
</script>

<style scoped>
  .profile-item {
    filter: drop-shadow(0 5px 10px rgba(0, 0, 0, 0.6));
    margin-top: 10px;
  }
  .profile-item:active {
    background-color: rgb(102, 102, 102);
  }
</style>