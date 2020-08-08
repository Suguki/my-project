<template>
  <div class="my-skills container-fluid h-100" id="my-skills">
    <h1>My Skills</h1>
    <br />
    <h3>Languages</h3>
    <div class="card-deck row">
      <div v-for="(cardItem, key) in cardItems" :key="key" class="col-md-4">
        <card v-bind="cardItem"  class="cursor img img-responsive" />
      </div>
    </div>
    <br />
    <br />
    <hr />
    <h3>Frameworks/Libraries</h3>
    <div class="card-deck row">
      <div v-for="(framework, key) in frameworks" :key="key" class="col-md-6">
        <card v-bind="framework" class="cursor img" />
      </div>
    </div>
    <br />
    <br />
    <hr />
    <h3>Others</h3>
    <div class="card-deck row">
      <div v-for="(other, key) in others" :key="key" class="col-md-6">
        <card v-bind="other" class="cursor img" />
      </div>
    </div>
    <br>
  </div>
</template>
<script>
import Card from "../atoms/Card";
export default {
  components: {
    Card,
  },
  data() {
    return {
      cardItems: [
        {
          title: "HTML&CSS",
          logo: 'images/HTML&CSS-logo.png',
          comment: "CSSライブラリであるBootStrapを用いて簡単なサイトデザインを作ることのできるレベルです.",
        },
        {
          title: "Java Script",
          logo:'images/JS-logo.png',
          comment: "簡単なDOM操作を利用し、小規模なアルゴリズムを1からかけるレベルです.Vue.jsを扱うにあたり最低限の基礎知識を持っています.",
        },
        {
          title: "php",
          logo:'images/php-logo.png',
          comment: "CRUD操作やログインページの実装(バリデーション含む)を1から一人で行うことができるレベルです.",
        },
      ],
      frameworks: [
        {
          title: "Laravel",
          logo: 'images/Laravel-logo.png'
            ,
          comment: "CRUD機能に加え、DBテーブルのリレーション管理、画像ファイルのアップロード機能の実装を一人で行うことができるレベルです.",
        },
        {
          title: "Vue.js",
          logo: 'images/Vue.js-logo.png',
          comment: "セレクトボックスやラジオボタン等のコンポーネントを自作し、当サイトページのようなものを作ることができるレベルです.",
        },
      ],
      others: [
        {
          title: "Docker",
          logo: 'images/Docker-logo.png',
          comment: "Dockerを使ってアプリの環境構築を行うことができるレベルです",
        },
        {
          title: "GitHub",
          logo: 'images/GitHub-logo.png',
          comment: "push&pull、marge&rebase、pullRequestなど、チーム開発にあたり必要な最低限の操作知識があります。Soucetreeを使っています.",
        },
      ],
    };
  },
};
</script>
<style scoped>
h1 {
  font-size: 70px;
}

.my-skills {
  height: 1300px;
  background-color: aqua;
}

.cursor {
  cursor: pointer;
}

.img {
  height: 250px;
}
</style>