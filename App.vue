<template>
  <div id="app">
    <Header></Header>
    <main>
      <div id="eyechatch">
        <p class="eyechatch-title">機械ではできない仕事を</p>
        <table class="news">
          <tr>
            <td>2019/01/01</td>
            <th rowspan="2">news</th>
          </tr>
          <tr>
            <td>ニュースタイトルがここに入ります。3月の決算報告書</td>
          </tr>
        </table>
      </div>
      <div id="mission">
        <div class="mission-contents">
          <h2>お客様のために進化する成長企業であり続ける</h2>
          <p>
            顧客主導型サービスを提供する企業として、お客様の会社経営に必要なサービスと情報を提供し続ける企業支援会社を目指します。企業が現在直面している「勝ち残る」の戦略を提供できる会社として、ホームページを始め、各種マーケティングを提供いたします。
          </p>
          <a href="#">ミッション詳細</a>
        </div>
        <div class="mission-img">
          <img src="./assets/mission-img.jpg" />
        </div>
      </div>
      <div id="service">
        <h2>service</h2>
        <div class="service1">
          <div class="service1-img">
            <img src="./assets/service2.jpg" />
          </div>
          <div class="service1-content">
            <h3>web製作事業</h3>
            <h4>コーチングのミッション</h4>
            <p>
              ユーザーから求めるものを分析し、ユーザビリティを備えた最適なサイトを提供。建設業から美容、ブライダル、飲食店まで多種多様な業種の製作実績があります
            </p>
            <div class="service-link">
              <a href="#" class="service1-link">サービス詳細</a>
            </div>
          </div>
        </div>
        <div class="service2">
          <div class="service2-img">
            <img src="./assets/service1.jpg" />
          </div>
          <div class="service2-content">
            <h3>web製作事業</h3>
            <h4>コーチングのミッション</h4>
            <p>
              ユーザーから求めるものを分析し、ユーザビリティを備えた最適なサイトを提供。建設業から美容、ブライダル、飲食店まで多種多様な業種の製作実績があります
            </p>
            <div class="service-link">
              <a href="#" class="service1-link">サービス詳細</a>
            </div>
          </div>
        </div>
      </div>
      <div id="company">
        <div class="flex-box">
          <div class="company">
            <h2>company</h2>
            <a href="#"></a>
            <p><b>会社概要</b></p>
          </div>
          <div class="recruit">
            <h2>recruit</h2>
            <a href="#"></a>
            <p><b>採用情報</b></p>
          </div>
        </div>
        <div class="question">
          <h2>FAQ</h2>
          <p>良くある質問</p>
          <div></div>
          <a href="#"></a>
        </div>
      </div>
      <div id="contact">
        <div class="contact-area">
          <h2>contact</h2>
          <h3>お問い合わせ</h3>
          <p class="contact-title">お気軽にお問い合わせください。</p>
          <p class="contact-content">
            資料請求・お問い合わせなど何でも気軽にお問い合わせください。お仕事のご連絡もお問い合わせページに飛んでいただいて、入力フォームにご記入お願いします。
          </p>
          <a href="#" class="contact-btn">お問い合わせへ</a>
        </div>
      </div>
        <button class="top_button" type="button" name="top_btn" @click="toppage">＞</button>
    </main>
    
    <Footer></Footer>
  </div>
</template>

<script>
import Header from "./components/CommonHeader";
import Footer from "./components/CommonFooter";

export default {
  methods: {
    toppage() {
      window.scrollTo({
        top: 0,
        left: 0,
        behavior: 'smooth'
      });
    }
  },
  components: {
    Header,
    Footer
  }
};
</script>

<style>
@charset "utf-8";

/* リセットcss */
html,
body,
div,
span,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
abbr,
address,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
samp,
small,
strong,
sub,
sup,
var,
b,
i,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section,
summary,
time,
mark,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  outline: 0;
  font-size: 100%;
  vertical-align: baseline;
  background: transparent;
}

body {
  line-height: 1;
}

article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
  display: block;
}

nav ul {
  list-style: none;
}

blockquote,
q {
  quotes: none;
}

blockquote:before,
blockquote:after,
q:before,
q:after {
  content: "";
  content: none;
}

a {
  margin: 0;
  padding: 0;
  font-size: 100%;
  vertical-align: baseline;
  background: transparent;
}

/* change colours to suit your needs */
ins {
  background-color: #ff9;
  color: #000;
  text-decoration: none;
}

/* change colours to suit your needs */
mark {
  background-color: #ff9;
  color: #000;
  font-style: italic;
  font-weight: bold;
}

del {
  text-decoration: line-through;
}

abbr[title],
dfn[title] {
  border-bottom: 1px dotted;
  cursor: help;
}

table {
  border-collapse: collapse;
  border-spacing: 0;
}

/* change border colour to suit your needs */
hr {
  display: block;
  height: 1px;
  border: 0;
  border-top: 1px solid #cccccc;
  margin: 1em 0;
  padding: 0;
}

input,
select {
  vertical-align: middle;
}

/* 共通のスタイル */
.section-title {
  font-size: 30px;
  font-weight: bold;
  margin: 30px 0;
  text-align: center;
}

img {
  display: block;
  width: 100%;
}

.wrap {
  width: 80%;
  margin: 0 auto 50px;
}

.flex {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.between {
  justify-content: space-between;
}

.around {
  justify-content: space-around;
}

#eyechatch {
  background-image: url(./assets/eyecatch.jpg);
  height: 700px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: space-between;
  position: relative;
}

.eyechatch-title {
  color: white;
  font-size: 60px;
  font-weight: bold;
  font-style: oblique;
  position: absolute;
  top: 50%;
  margin: 0 0 0 150px;
}

.news {
  position: absolute;
  bottom: 0;
  right: 0;
  height: 60px;
  border-collapse:collapse;
}

.news th {
  background-color: black;
  color: white;
  line-height: 60px;
  padding: 0 50px;
  font-size: 14px;
}

.news td {
  background-color: white;
  color: black;
  width: 600px;
  padding-bottom: 20px;
}




#mission {
  background-color: black;
  position: relative;
  margin-bottom: 10%;
  z-index: 900;
}

.mission-contents {
  color: white;
  width: 50%;
  padding: 10% 0 10% 15%;
}

.mission-contents h2 {
  font-size: 25px;
  padding: 10px 0;
}

.mission-contents p {
  font-size: 14px;
  padding: 10px 0;
}

.mission-contents a {
  display: inline-block;
  padding: 10px 15px;
  margin: 20px 0;
  color: black;
  background-color: white;
  text-decoration: none;
  border-radius: 3px;
}

.mission-img img{
  margin: 20px;
  width: 40%;
  position: absolute;
  bottom: -15%;
  right: 3%;
  z-index: -900;
}

#service {
  height: 50%;
  background-color: rgb(197, 191, 191);
}

#service h2 {
  font-size: 30px;
  padding: 10px 0;
  text-align: center;
}

.service1 {
  display: block;
  position: relative;
  margin-bottom: 40%;
  height: 30%;
}

.service1-content {
  position: absolute;
  width: 35%;
  background-color: white;
  padding: 5% 5% ;
  margin-top: 5%;
  top: 20%;
  left: 18%;
  z-index: 2;
}

.service1-img img {
  width: 50%;
  margin-left: 50%;
  position: absolute;
  top: 10%;
  right: 0;
}

.service2 {
  display: block;
  position: relative;
  height: 670px;
}

.service2-content {
  width: 40%;
  background-color: white;
  padding: 60px 50px;
  position: absolute;
  top: 20%;
  right: 15%;
  z-index: 2;
}

.service2-img img {
  width: 50%;
  position: absolute;
  top: 10%;
  left: 0;
}

.service1 h3,
.service2 h3 {
  padding: 10px 0;
  font-size: 14px;
}

.service1 h4,
.service2 h4 {
  font-weight: normal;
  font-size: 14px;
  padding: 10px 0;
}

.service1 p,
.service2 p {
  padding: 10px 0;
  font-size: 13px;
}



.service-link {
  text-align: right;
}

.common-btn {
  display: block;
  width: 130px;
  height: 40px;
  line-height: 40px;
  background: #fff;
  padding: 0 20px;
  color: #000;
  text-align: center;
}

.service1-link {
  border: 0.5px solid black;
  padding: 8px 20px;
  display: inline-block;
  margin-top: 20px;
  color: black;
  font-size: 13px;
  text-decoration: none;
}


.flex-box {
  display: flex;
  justify-content: space-between;
}

.company,
.recruit {
  width: 47%;
  margin: 150px 0;
  text-align: center;
  padding: 100px 0;
  color: white;
}

.company h2,
.recruit h2 {
  font-size: 30px;
  padding-bottom: 10px;
}

.company {
  background-image: url(./assets/company.jpeg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  position: relative;
}

.company a {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.recruit {
  background-image: url(./assets/recruit.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  position: relative;
}

.recruit a {
  position: absolute;
  top: 0;
  right: 0;
  width: 100%;
  height: 100%;
}

.question {
  background-color: black;
  color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: relative;
  width: 80%;
  margin: 0 auto 150px;
  padding: 50px 0;
}

.question h2 {
  font-size: 30px;
  padding-left: 50px;
}

.question p {
  padding-right: 10%;
}

.question a {
  position: absolute;
  top: 0;
  right: 0;
  width: 100%;
  height: 100%;
}

#contact {
  color: white;
  background-image: url(./assets/contact-bg.jpg);
  /* height: 500px; */
  width: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

.contact-area {
  height: 100%;
  text-align: center;
}

#contact h2 {
  font-size: 30px;
  padding-top: 90px;
}

#contact h3 {
  padding: 15px 0;
}

.contact-title {
  font-size: 30px;
  padding: 10px 15%;
}

.contact-content {
  font-size: 13px;
  padding: 15px 10%;
}

.contact-btn {
  border: 2px solid white;
  padding: 8px 20px;
  display: inline-block;
  margin-top: 20px;
  color: white;
  font-size: 13px;
  text-decoration: none;
}

.top_button {
  color:white;
  background-color: rgba(132, 133, 131, 0.596);
  position: fixed;
  top: 92%;
  right: 2%;
  z-index:950;
  font-size: 15px;
  border-radius: 80px;
  border: none;
  transform: rotate(-90deg);
  width: 60px;
  height: 60px;
  }
.top_button:hover {
  background-color: black;
  transition: 0.8s;
}

@media screen and (max-width: 768px) {
    .eyechatch-title {
    top: 30%;
    margin: 0 auto;
    padding: 0 5%;
    text-align: center;
  }

  .news td {
    border: 1px solid white;
  }

  .mission-contents {
    margin: 0 auto;
    width: 70%;
    top: 3%;
    padding: 10% 0 10% 0;
    padding-top: 30px;
  }


  #mission-img {
    display: block;
  }


  .service1 {
    position: static;
    height: 30%;
    margin: 10% 0 15%;
  }

  .service2 {
    position: static;
    padding: 15% 0;
    height: 30%;
  }

  .service1-content,
  .service2-content {
    position: static;
    margin: 0 auto;
    padding: 5% 5% ;
    width: 70%;
  }


  /* .service1-img ,
  .service2-img  {
    margin: 0 auto;
    width: 100%;
  } */

  .service1-img img,
  .service2-img img {
    position: static;
    margin: 0 auto;
    width: 80%;
  }



  .flex-box {
    display: flex;
    justify-content: space-between;
    flex-wrap:wrap;
  }

  .company,
  .recruit {
    width: 100%;
    margin: 0;
  }

  .question {
    margin: 20px auto;
    width: 90%;
  }
}
</style>
