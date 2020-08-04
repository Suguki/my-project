<template>
  <div class="my-portfolio container" id="my-portfolio">
    <h1>My Portfolio</h1>
    <div class="card-deck row">
      <div class="col-md-6">
        <b-card
          title="pigGame"
          img-src="images/my-icon.JPG"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2 mx-auto"
        >
          <b-button v-b-modal.PigGameModal>詳細</b-button>

          <b-modal id="PigGameModal" title="PigGame">
            <div class="my-4">
              <ul>
                <li>概要：二人でサイコロを振り、どちらが早く出た目の合計が100になるか競うゲーム.意外とゲーム性あります.</li>
                <li>使用言語：JavaScript</li>
                <li>Github URL：</li>
                <li>使用環境:</li>
              </ul>
            </div>
          </b-modal>
        </b-card>
      </div>
      <div class="col-md-6 content-center">
        <b-card
          title="今日どこ行く？"
          img-src="images/pig_game.png"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2 mx-auto"
        >
          <b-button v-b-modal.KyodokoikuModal>詳細</b-button>

          <b-modal id="KyodokoikuModal" title="今日どこ行く？">
            <div class="my-4">
              <ul>
                <li>概要：休日何かしたいけど何しようかな...そんなときはこのアプリで案を出すのもいいのではないでしょうか.気分に沿って案を出してくれます。割と細かく案を絞れます。</li>
                <li>使用言語：PHP</li>
                <li>Github URL：</li>
                <li>使用環境: Docker/MySQL/nginex</li>
              </ul>
            </div>
          </b-modal>
        </b-card>
      </div>
    </div>
    <br>
    <br>
    <div class="card-deck row">
      <div class="col-md-6 text-center">
        <b-card
          title="TripCoffee"
          img-src="images/pig_game.png"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2 mx-auto"
        >
          <b-button v-b-modal.TripCoffeeModal>詳細</b-button>

          <b-modal id="TripCoffeeModal" title="TripCoffee">
            <div class="my-4">
              <ul>
                <li>概要：カフェ好きが高じて誕生しました.今日どこ行く？</li>
                <p>とは違いレビューや店の評価ができます.</p>
                <li>使用言語：PHP/Laravel</li>
                <li>Github URL：</li>
                <li>使用環境: Docker/MySQL/nginex</li>
              </ul>
            </div>
          </b-modal>
        </b-card>
      </div>
    </div>
  </div>
</template>

<style scoped>
.my-portfolio {
  height: 800px;
  background-color: palevioletred;
}
</style>