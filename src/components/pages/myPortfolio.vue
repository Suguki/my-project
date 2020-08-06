<template>
  <div class="my-portfolio container-fluid h-100" id="my-portfolio">
    <h1>My Portfolio</h1>
    <div class="card-deck row">
      <div class="col-md-6">
        <b-card
          title="pigGame"
          img-src="images/pig_game.png"
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
                <li><span class="font-weight">概要：</span>二人でサイコロを振り、どちらが早く出た目の合計が100になるか競うゲーム。意外とゲーム性あります。</li>
                <li><span class="font-weight">使用言語</span>JavaScript/HMTL/CSS<br>
                DOM操作を利用し、ページ遷移することなくアクションを実行するため、JavaScriptを使用し作成しました。
                </li>
                <li><span class="font-weight">使用環境</span></li>
                <li><a href="#">Githubページへ</a></li>
              </ul>
            </div>
          </b-modal>
        </b-card>
      </div>
      <div class="col-md-6 content-center">
        <b-card
          title="今日どこ行く？"
          img-src="images/whereAreYouGoToday.png"
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
                <li><span class="font-weight">概要：</span>休日何かしたいけど何しようかな...そんなときはこのアプリで案を出すのもいいのではないでしょうか。
                気分に沿って案を出してくれます。割と細かく案を絞れます。</li>
                <li><span class="font-weight">使用言語：</span>HTML/CSS/Bootstrap/PHP<br>
                アプリの機能を実装するに当たり、DBを使ったバックエンド処理が必要であったためphpを使用し作成しました。</li>
                <li><span class="font-weight">使用環境: </span>Docker/MySQL/nginx</li>
                <li><a target="_blank" href="https://github.com/Suguki/kyodokoiku">Githubページへ</a></li>
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
          img-src="images/Trip-Coffee.png"
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
                <li><span class="font-weight">概要：</span>カフェ好きが高じて誕生しました.今日どこ行く？</li>
                <p>とは違いレビューや店の評価ができます.</p>
                <li><span class="font-weight">使用言語：</span>HTML/CSS/Bootstrap/PHP/Laravel
                <br>今日どこ行く？を作成phpの基礎をしある程度学んだので、フレームワークを利用しもう少しリッチなアプリを作成したいと思いLaravelを使いました。</li>
                <li><span class="font-weight">使用環境：</span> Docker/MySQL/nginx</li>
                <li><a href="https://github.com/Suguki/cafe_review" target="_blank">Githubページへ</a></li>
              </ul>
            </div>
          </b-modal>
        </b-card>
      </div>
    </div>
  </div>
</template>

<style scoped>
h1 {
  font-size: 70px;
}

.my-portfolio {
  height: 850px;
  background-color: palevioletred;
}

.font-weight {
  font-weight: bolder;
}
</style>