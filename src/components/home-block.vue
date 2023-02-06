<template>
  <div class="container">
    <my-nav />

    <div class="contents">
      <div class="title">Bilgi <br />Teknolojilerinde <br />23 Yıllık Tecrübe</div>
      <div class="content">
        Müşterilerimizin yüksek kalite seviyelerini koruyabilmeleri için farklı sektörlerde tecrübe kazanmış uzman<br />
        kadrolarımızla Proje Yönetimi, İş Analizi ve Test Yönetimi hizmetleri sunmaktayız.
      </div>
    </div>

    <div>
      <div class="mail">
        <div>
          <input type="text" placeholder="Mail bültenimize kayıt ol" />
        </div>
        <my-button modifier="mailsend">Kayıt Ol</my-button>
      </div>
    </div>
  </div>
</template>

<script setup>
import MyNav from "./my-nav.vue"
import MyButton from "./my-button.vue"
</script>

<style scoped>
.container {
  background-image: radial-gradient(circle at 141% 78%, #fff, rgba(255, 255, 255, 0) 107%), url("@/assets/images/rectangle-1.jpg");
  background-size: cover;
  height: 754px;
  background-position: right 35% bottom 45%;
  width: 100%;
}

.items > div:hover {
  cursor: pointer;
  color: #0f29e8;
}
.contents {
  text-align: center;
  width: 100%;
}
.title {
  font-size: 40px;
}
.content {
  font-size: 12px;
  line-height: 1.92;
}
.mail {
  display: flex;
  background-color: #fff;
  border-radius: 5px;
  justify-content: space-between;
  padding: 10px;
  align-items: center;
  margin: 10px;
}
.mail input {
  outline: none;
  border: none;
  color: rgba(0, 0, 0, 0.4);
  padding-left: 15px;
}

@media (min-width: 375px) and (max-width: 1023px) {
  .items {
    display: none;
  }
  .hamburger {
    visibility: visible;
  }

  .line {
    border: 1px solid black;
    width: 20px;
  }
  .line:nth-child(2),
  .line:nth-child(3) {
    margin-top: 5px;
  }
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .container {
    background-image: url("@/assets/images/rectangle-1.jpg");
    height: 100vh;
    background-position: 0px 0px;
  }
  .hamburger {
    display: none;
  }

  .box {
    display: flex;
    margin: 30px;
  }
  .box div {
    margin-right: 25px;
  }
  .items {
    display: flex;
    align-items: center;
  }

  .title {
    font-size: 62px;
    text-align: left;
    margin-left: 122px;
  }
  .title br:nth-child(1) {
    display: none;
  }
  .content {
    margin-top: 20px;
    line-height: 1.8;
    font-size: 19px;
    text-align: left;
    margin-left: 122px;
  }
  .mail {
    display: flex;
    background: #fff;
    width: 502px;
    border-radius: 8px;
    justify-content: space-between;
    padding: 6px 6px 6px 32px;
    margin: 30px 163px 0 0;
    margin-left: 122px;
  }
  .mail input {
    border: none;
    outline: none;
    align-items: center;
    margin: 13px 150px 12px 0;
  }
}
@media (min-width: 1440px) {
  .container {
    background-image: url("@/assets/images/rectangle-1.jpg");
    background-position: 50% 50%;
  }

  .hamburger {
    display: none;
  }

  .box {
    margin: 50px;
    margin-right: 0px;
  }
  .box div {
    margin-right: 25px;
  }
  .items {
    display: flex;
    align-items: center;
  }

  .title {
    font-size: 62px;
    text-align: left;
    margin-left: 122px;
  }
  .title br:nth-child(1) {
    display: none;
  }
  .content {
    margin-top: 20px;
    line-height: 1.8;
    font-size: 19px;
    text-align: left;
    margin-left: 122px;
  }
  .mail {
    width: 502px;
    padding: 6px 6px 6px 32px;
    margin: 30px 163px 0px 0;
    margin-left: 122px;
  }
  .mail input {
    margin: 13px 150px 12px 0;
  }
}
</style>
