<template>
  <div id="app">
    <nav-bar></nav-bar>
    <my-Profile></my-Profile>
    <mySkills></mySkills>
    <myPortfolio></myPortfolio>
    <div class="position">
      <scroll-btn></scroll-btn>
    </div>
  </div>
</template>

<script>
import mySkills from "./components/pages/mySkills";
import myProfile from "./components/pages/myProfile";
import myPortfolio from "./components/pages/myPortfolio";
import NavBar from "./components/atoms/NavBar";
import ScrollBtn from "./components/atoms/ScrollBtn";

export default {
  components: {
    myProfile,
    mySkills,
    myPortfolio,
    NavBar,
    ScrollBtn

  },
  data() {
    return {
      drawer: false,
    };
  },
};
</script>
<style scoped>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 40px;
}
#my-profile {
  padding-top: 40px;
}
#my-skills {
  padding-top: 40px;
}
#my-portfolio {
  padding-top: 40px;
}
.position {
  position: fixed;
  bottom: 5px;
  right: 5px;
}
</style>

