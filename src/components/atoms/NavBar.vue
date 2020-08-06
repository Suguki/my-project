<template>
  <div>
    <nav class=" container-fluid navbar navbar-expand navbar-dark bg-dark fixed-top">
      <div
        class="collapse navbar-collapse justify-content-center custom-nav"
        id="navbarSupportedContent"
      >
        <div class="navbar-nav">
          <a v-scroll-to="'#my-profile'">My Profile</a>
          <a v-scroll-to="'#my-skills'">My Skills</a>
          <a v-scroll-to="'#my-portfolio'">My Portfolio</a>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>


export default {
  components: {

  },
  data() {
    return {
      drawer: true,
    };
  },
  methods: {
    toTop() {
      this.drawer = false;
      this.$router.push({ name: "top" }).catch(() => {});
    },
    toTerm() {
      this.drawer = false;
      this.$router.push({ name: "term" }).catch(() => {});
    },
    toPrivacyPolicy() {
      this.drawer = false;
      this.$router.push({ name: "privacy_policy" }).catch(() => {});
    },
  },
};
</script>

<style scoped>
.navbar {
  height: 60px;
  filter: drop-shadow(0 5px 10px rgba(0, 0, 0, 0.6));
}

.custom-nav {
  overflow-x: scroll;
  overflow-y: hidden;
  flex-wrap: nowrap;
}
.navbar-nav {
  height: 40px;
  color: aliceblue;
}

.navbar-nav a {
  width: 100px;
  padding-top: 9px;
  padding-bottom: 10px;
}
.navbar-nav a:hover {
  background-color: darkgray;
}
</style>