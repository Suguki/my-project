<template>
  <div class="my-profile container-fluid h-100" id="my-profile">
    <div>
      <h1>My Profile</h1>
    </div>
    <br />
    <br />
    <div class="row">
      <div class="col-md-7">
        <ul>
          <li>
            <h5 class="font-weight">名前:</h5>
          </li>
          <p class="space">藤田 佑真</p>
          <br />
          <li>
            <h5 class="font-weight">前職：</h5>
          </li>
          <p class="space">
            メック株式会社 研究開発本部 技術開発センター
            <br />化学メーカーで電子基板の製造工程に用いられる薬液の開発をしていました。
          </p>
        </ul>
      </div>
      <div class="col-md-5 img-edge">
        <img src="images/my-icon.JPG" class="img" />
      </div>
    </div>
    <br />
    <div claaa="row">
      <div class="col-md-12 h-100 parallel">
        <ul class="col-md-12">
          <li>
            <h5 class="font-weight">自己紹介：</h5>
          </li>
          <p class="space">
            2019年4月に化学メーカーであるメック株式会社へ入社し、研究開発員として基板関連製品の開発に携わってきました。
            2020年6月末日を以て退職し、現在に至ります。
            勤務地は近畿圏内を希望しています。
            業界未経験ではありますが、業務時間外の勉強を惜しまず、いち早く業務に馴染めるよう食らいついてく所存です。
          </p>
          <br />
          <li>
            <h5 class="font-weight">自身の強み・実績</h5>
          </li>
          <p class="space">
            学生時代の部活動
            <br />・中高6年間を通してソフトテニス部に所属し、中学では団体で京都府優勝、高校では個人戦で市内ベスト4の実績があります。
            <br />・中学では全国大会出場経験のあるジュニア選手が半数を占める中未経験で入部し、3年生でレギュラー入りし上記の実績を
            残すことができました。
            <br />・実績を残すことができた理由にもつながるのですが、一度熱が入ると一日中そのことについて考えるタイプであることが
            強みです。
            <br />
          </p>
          <br />
          <li>
            <h5 class="font-weight">専攻分野:</h5>
          </li>
          <p class="space">
            ・前職で培った電子基板業界の知識があります。
            <br />・学生時代は分子生物学、免疫学、遺伝子工学について専攻していました。余談ですが、新型コロナウイルス検査に用いられる
            PCR検査についても精通しています。
            <br />・また学生時代、前職では特にコミュニケーションに気を配ってきました。研究生活では自身のタスク進行状況がクローズになる
            傾向があるため、常に周りに対し、仕事の見える化を意識して取り組んできました。それに加え前職では顧客と直接やり取りを
            行いながら新製品のプレゼン、導入に携わった経験もあり、社会人としてコミュニケーションの基礎はしっかり身につけている
            という自負があります。
          </p>
          <br />
          <li>
            <h5 class="font-weight">この先やってみたいこと:</h5>
          </li>
          <p class="space">
            フロント、バックエンドどちらにも強い興味がありますが、まずはバックエンドの開発業務に携わりたいと考えています。
            理由としては、バックエンドで設計やセキュリティ対策についてより深く学びたいという気持ちがあるためです。
          </p>
          <br />
          <li>
            <h5 class="font-weight">最後に:</h5>
          </li>
          <p class="space">
            WEBエンジニアとしての開発業務に強い好奇心はありますが、まずは自社の製品、サービスに愛を持って仕事をして
            いきたいです。前職での経験をもとに、貴社のビジネスに対して愛が持てそうか、という観点を大事に求職活動をさせて頂いて
            おります。採用いただけましたら貴社の事業拡大に貢献すべく、精一杯努力していくつもりです。
            以上、よろしくお願いいたします。
          </p>
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

.img {
  display: block;
  height: auto;
  max-width: 100%;
  position: absolute;
  top: 30%;
  left: 50%;
  margin-right: -50%;
  transform: translate(-50%, -50%);
}

.img-edge img {
  border-radius: 100px;
  vertical-align: middle;
}

.font-weight {
  font-weight: bolder;
}
</style>