<template>
  <div class="my-profile container" id="my-profile">
    <div class>
      <h1>My Profile</h1>
    </div>
    <div class="row">
      <div class="col-xs-12 col-md-4 parallel img-edge">
        <img src="images/my-icon.JPG" />
      </div>
      <div class="col-xs-12 col-md-8 parallel">
        <ul>
          <li>名前:</li>
          <p class="space">藤田 佑真</p>

          <li>前職：</li>
          <p class="space">メック株式会社 研究開発本部 技術開発センター<br>
            化学メーカーで電子基板の製造工程に用いられる薬液の開発をしていました。</p>
          <li>自己紹介：</li>
          <p class="space">2019年4月に化学メーカーであるメック株式会社へ入社し、研究開発員として基板関連製品の開発に携わってきました。
              2020年6月末日を以て退職し、現在に至ります。
              勤務地は近畿圏内を希望しています。
              業界未経験ではありますが、業務時間外の勉強を惜しまず、いち早く業務に馴染めるよう食らいついてく所存です。</p>
          <li>この先やってみたいこと:</li>
          <p class="space">フロント、バックエンドどちらにも強い興味がありますが、まずはバックエンドの開発業務に携わりたいと考えています。
              理由としては、バックエンドで設計やセキュリティ対策についてより深く学びたいという気持ちがあるためです。</p>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
h1 {
  font-size: 70px;
}
.my-profile {
  height: 600px;
  background-color: greenyellow;
}

.parallel {
  display: inline-block;
  height: 400px;
}

ul {
  text-align: left;
}

.space {
  margin: 0px;
}

.img-edge img{
  border-radius: 100px;
}
</style>