<template>
  <div class="my-skills container" id="my-skills">
    <h1>My Skills</h1>
    <div class="card-deck row">
      <div v-for="(cardItem, key) in cardItems" :key="key" class="col-xs-12 col-md-6">
        <card v-bind="cardItem" />
      </div>
    </div>
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
          title: "php",
          description:
            "CRUD操作や入力ページの実装を1から一人で行うことができるレベルです.",
          comment: "comment1",
        },
        {
          title: "Java Script",
          description:
            "簡単なDOM操作を利用し、小規模なアルゴリズムを1からかけるレベルです.またapiの実装などもできます.",
          comment: "comment2",
        },
        {
          title: "Lravel",
          description:
            "CRUD操作に加え、リレーションテーブルを用いた簡単なアプリを1から一人で実装できるレベルです.",
          comment: "comment3",
        },
        {
          title: "Vue.js",
          description:
            "コンポーネント間のデータ受け渡しやVue-routerなどの基礎知識を利用し、サイトのページの構築を行うことができます.",
          comment: "comment4",
        },
      ],
    };
  },
};
</script>
<style scoped>
.my-skills {
  height: 1000px;
  background-color: aqua;
}
</style>