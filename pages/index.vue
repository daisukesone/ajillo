<template>
    <section>
<header>
  <nav>
  <div class="nav-wrapper">
    <div class="logo"></div>
  <div class="nav-menu">
    <a class="nav-items" href="#about">about</a>
    <a class="nav-items" href="information">information</a>
    <a class="nav-items" href="contact">contact</a>
    <div class="nav-items instagram-logo"></div>
    <div class="nav-items youtube-logo"></div>
  </div>
  </div>
  </nav>
  <div class="fv">
  <div class="fv-image"></div>
  <div class="fv-frame"></div>
  </div>


</header>
<section class="about" id="about">
<h1 class="about-title">Share Happy Time &amp; Emotion</h1>
<h1 class="about-subtitle">ヒトとヒトが同じ感情をシェアする時間の量と質を最大化したい</h1>
<p classs="about-message">あなたはだれかと同じ気持ちをシェアして仲が深まったことはありませんか<br>
友達の家で食べた手づくりの料理、仕事帰りのお店で食べたあの料理<br>
ささやかだけれど、しあわせの詰まった時間を誰かとシェアすることで、<br>
お互いのココロが近づき、結びついたような感覚になれる<br>
そして気兼ねなく色々なこと伝え合えるようになる<br><br><br>

アヒージョにも、<br>
小さな器の中にやさしくてしあわせな時間が詰まっています<br>
溢れています<br>
</p>
</section>
<section class="information" id="information">
  <div class="information-left">
    <img src="../assets/images/demo_top.png" alt="" width="475px">
    <img src="../assets/images/demo_top.png" alt="" width="475px">
  </div>
  <div class="information-right">
    <h1>information</h1>
    <p>テキストテキストストテキストテキストテキストテキストテキストストテキストテキストテキストテキストテキストストテキストテキストテキストテキストテキストストテキストテキストテキストテキストテキストストテキストテキストテキスト</p>
  </div>
</section>
<section class="instagram">
  <div class="flex">
<div class="instagram-logo"></div>
  <h1>instagram</h1>
  </div>
  <div class="instagram-posts">
    <img src="../assets/images/posts_1.png" alt="" width="263px">
    <img src="../assets/images/posts_2.png" alt="" width="263px">
    <img src="../assets/images/posts_3.png" alt="" width="263px">
    <img src="../assets/images/posts_4.png" alt="" width="263px">
  </div>
  <div style="text-align: right;"><a href="https://instagram.com/hatopo_ajillo">more</a></div>
</section>
<section class="youtube">
  <div class="flex">
<div class="youtube-logo"></div>
  <h1>Youtube</h1>
  </div>
  <p>coming soon...</p>
</section>

<section id="contact">
  <h1>contact</h1>
    <div class="p-contact">
    <form class="p-contact__form" name="contact" method="POST" data-netlify="true" data-netlify-honeypot="bot-field" @submit.prevent="onSubmit" :class="sendingClass">
      <input type="hidden" name="form-name" value="contact">

      <div class="p-contact__item">
        <label for="username">お名前</label>
        <input type="text" id="username" name="username" v-model="username" autocomplete="name">
      </div>
      <!-- /.p-contact__item -->

      <div class="p-contact__item">
        <label for="katakana">フリガナ</label>
        <input type="text" id="katakana" name="katakana" v-model="katakana">
      </div>
      <!-- /.p-contact__item -->

      <div class="p-contact__item">
        <label for="useremail">メールアドレス</label>
        <input type="text" id="useremail" name="useremail" v-model="useremail" autocomplete="email">
      </div>
      <!-- /.p-contact__item -->

      <div class="p-contact__item">
        <label for="message">お問い合わせ内容</label>
        <textarea id="message" name="message" v-model="message"></textarea>
      </div>
      <!-- /.p-contact__item -->

      <div class="p-contact__item" v-show="false">
        <label for="message">スパムでない場合は空欄</label>
        <input type="text" name="bot-field" v-model="botField"/>
      </div>
      <!-- /.p-contact__item -->

      <div class="p-contact__submit">
        <button type="submit">送信</button>
      </div>
      <!-- /.p-contact__submit -->
    </form>
    <!-- /.p-contact__form -->
  </div>
  </div>
</section>
</section>
</template>



<script>
export default {}
</script>

<style>

header{
  width: 100%;
  position: relative;
}
.container {
  margin: 0 auto;
  min-height: 100vh;
  width: 98%;
  /* display: flex; */
  justify-content: center;
  align-items: center;
  text-align: center;
}

.nav{
  height: 100%;
}

.nav-wrapper{
  padding-top: 16px;
  display: flex;
  justify-content: space-between;
  max-width: 1170px;
  margin: 0 auto;
  align-items: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}


.image{
  width: 100%;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

* {
  box-sizing: border-box;
}
body {
  font-size: 14px;
}

a:hover{
  text-decoration: none;
  color: #000;
}

.flex{
  display: flex;
  align-items: center;
  justify-content: center;
}

.fv{
  height: 686px;
  max-width: 1170px;
  margin: 0 auto;
  position: relative;
}

.fv-image {
  width: 98%;
  height: 654px;
  background: url("~@/assets/images/fv-image.png");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  opacity: 1;
  overflow: hidden;
  position: absolute;
  top: 0;
  left: 0;
}

.fv-frame{
width: 98%;
height: 654px;
border: #000 solid 1px;
position: absolute;
  bottom: 0;
  right: 0;
  z-index: -1;
}

.v301_25 {
  width: 100%;
  height: 670px;
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  opacity: 1;
  position: absolute;
  top: 125px;
  left: 98px;
  border: 1px solid rgba(0,0,0,1);
  overflow: hidden;
}
.about {
  margin: 0 auto;
  max-width: 1170px;
    color: rgba(0,0,0,1);
    font-family: Jost,YuGothic;
    /* font-weight: Bold; */
    /* font-size: 20px; */
  line-height: 46px;
  letter-spacing: 0.1em;
  text-align: center;
}

.about-title{
  margin-top: 125px;
font-style: normal;
font-weight: bold;
font-size: 32px;
}

.about-subtitle{
  font-weight: bold;
font-size: 20px;
line-height: 30px;
letter-spacing: 0.1em;
}
.about p{
  font-family: YuGothic;
font-style: normal;
font-weight: 500;
font-size: 20px;
line-height: 47px;
text-align: center;
letter-spacing: 0.1em;
}

.about-message{
  margin-top: 74px;
}

.nav-menu{
  display: flex;
    align-items: center;
}

.nav-items{
  color: rgba(0,0,0,1);
  font-family: Jost;
  font-size: 24px;
  margin: 0 15px;

}
.v703_1 {
  width: 547px;
  color: rgba(0,0,0,1);
  position: absolute;
  top: 920px;
  left: 442px;
  font-family: Jost;
  font-weight: Bold;
  font-size: 32px;
  opacity: 1;
  text-align: left;
}
.v302_30 {
  width: 192px;
  color: rgba(0,0,0,1);
  position: absolute;
  top: 2746px;
  left: 638px;
  font-family: Jost;
  font-weight: Bold;
  font-size: 32px;
  opacity: 1;
  text-align: left;
}
.v304_8 {
  width: 234px;
  color: rgba(0,0,0,1);
  position: absolute;
  top: 1994px;
  left: 886px;
  font-family: Jost;
  font-weight: Bold;
  font-size: 32px;
  opacity: 1;
  text-align: left;
}
.v302_37 {
  width: 182px;
  color: rgba(0,0,0,1);
  position: absolute;
  top: 3287px;
  left: 1202px;
  font-family: Jost;
  font-weight: Regular;
  font-size: 32px;
  opacity: 1;
  text-align: left;
}
.v301_27 {
  width: 752px;
  color: rgba(0,0,0,1);
  position: absolute;
  top: 1095px;
  left: 344px;
  font-family: YuGothic;
  font-weight: Medium;
  font-size: 20px;
  opacity: 1;
  text-align: center;
}
.v703_32 {
  width: 650px;
  color: rgba(0,0,0,1);
  position: absolute;
  top: 991px;
  left: 395px;
  font-family: YuGothic;
  font-weight: Bold;
  font-size: 20px;
  opacity: 1;
  text-align: left;
}
.v302_32 {
  width: 575px;
  color: rgba(0,0,0,1);
  position: absolute;
  top: 2118px;
  left: 718px;
  font-family: YuGothic;
  font-weight: Medium;
  font-size: 28px;
  opacity: 1;
  text-align: left;
}
.information {
  margin: 0 auto;
  margin-top: 167px;
  max-width: 1170px;
    color: rgba(0,0,0,1);
    font-family: Jost,YuGothic;
    /* font-weight: Bold; */
    /* font-size: 20px; */
  line-height: 46px;
  letter-spacing: 0.1em;
  text-align: center;
  display: flex;
}
.information-left{
  width: 50%;
}
.information-right{
  width: 50%;
}

.contact {
  width: 98px;
  color: rgba(0,0,0,1);
  font-family: Jost;
  font-weight: Regular;
  font-size: 24px;
  text-align: left;
}


.instagram-logo {
  display: inline-block;
  overflow: hidden;
  width: 28px;
  height: 28px;
  background: url("~@/assets/images/instagram.png");
  background-size: cover;
  opacity: 1;
}

.instagram{
margin-top: 167px;
margin-right: auto;
margin-left: auto;
max-width: 1170px;
}


.instagram  h1{
      margin-left: 8px;
  font-family: Jost;
font-style: normal;
font-weight: bold;
font-size: 32px;
line-height: 46px;
letter-spacing: 0.1em;
}

.instagram a {
  color: #000;
      text-align: right;
    padding-right: 48px;
  font-family: Jost;
font-style: normal;
font-weight: normal;
font-size: 32px;
line-height: 46px;
letter-spacing: 0.1em;
}

.instagram-posts{
  margin: 0 auto;
  display: flex;
      justify-content: center;
}

.instagram-posts img{
  margin: 5px;
}

.youtube{
margin-top: 167px;
margin-right: auto;
margin-left: auto;
max-width: 1170px;
}

.youtube-logo {
  display: inline-block;
  width: 45px;
  height: 45px;
    background: url("~@/assets/images/youtube.png");
  background-size: cover;
}

.youtube h1{
      margin-left: 8px;
font-family: Jost;
font-style: normal;
font-weight: bold;
font-size: 32px;
line-height: 46px;
letter-spacing: 0.1em;
}

.youtube p{
  margin-top: 32px;
  text-align: center;
    color: #000;
  font-family: Jost;
font-style: normal;
font-weight: normal;
font-size: 32px;
line-height: 46px;
letter-spacing: 0.1em;
}

#contact{
  margin-top: 167px;
margin-right: auto;
margin-left: auto;
max-width: 1170px;

}

#contact h1{
  text-align: center;
font-family: Jost;
font-style: normal;
font-weight: bold;
font-size: 32px;
line-height: 46px;
letter-spacing: 0.1em;
}

.logo {
  width: 76px;
  height: 68px;
  background: url("~@/assets/images/logo.png");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  overflow: hidden;
}

.p-contact{
text-align: center;
}

.p-contact__item{
  display: flex;
flex-direction: column;
align-items: flex-start;
padding: 12px;
color: #7A7F8C;
}

input{
  background: #F8FAFC;
border-radius: 4px;
border: #F8FAFC;
    width: 320px;
}
textarea{
    background: #F8FAFC;
border-radius: 4px;
border: #F8FAFC;
    width: 320px;
}

</style>
