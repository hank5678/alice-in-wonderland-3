<template>
  <div class="container">
    <div class="navs">
      <div class="hamburger">
        <div class="line line1"></div>
        <div class="line line2"></div>
        <div class="line line3"></div>
      </div>
      <div class="box">
        <div class="items">
          <div>Çözüm ve Hizmetler</div>
          <div>Ürünler</div>
          <div>Teknolojiler</div>
          <div>İnsan Kaynakları</div>
          <div>Kurumsal</div>
        </div>
        <div class="redbutton">İletişim</div>
      </div>
    </div>

    <div class="contents">
      <div class="title">Bilgi <br />Teknolojilerinde <br />23 Yıllık Tecrübe</div>
      <div class="content">
        Müşterilerimizin yüksek kalite seviyelerini koruyabilmeleri için farklı sektörlerde tecrübe kazanmış uzman<br />
        kadrolarımızla Proje Yönetimi, İş Analizi ve Test Yönetimi hizmetleri sunmaktayız.
      </div>
      <div class="mail">
        <div>
          <input type="text" placeholder="Mail bültenimize kayıt ol" />
          <div class="redbutton mailsend">Kayıt Ol</div>
        </div>
      </div>
    </div>
    <div class="contents1">
      <div class="title">
        Bilgi Teknolojilerinde<br />
        23 Yıllık Tecrübe
      </div>
      <div class="content">
        Müşterilerimizin yüksek kalite seviyelerini koruyabilmeleri için farklı<br />
        sektörlerde tecrübe kazanmış uzman kadrolarımızla Proje Yönetimi, İş<br />
        Analizi ve Test Yönetimi hizmetleri sunmaktayız.
      </div>
      <div class="mail">
        <div>
          <input type="text" placeholder="Mail bültenimize kayıt ol" />
          <div class="redbutton mailsend">Kayıt Ol</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.container {
  background-image: radial-gradient(circle at 141% 78%, #fff, rgba(255, 255, 255, 0) 107%), url("@/assets/images/rectangle-1.jpg");

  background-size: cover;
  background-position: right 35% bottom 45%;
  width: 100%;
}
.line1 {
  border: 1px solid black;
  width: 20px;
}
.line2 {
  border: 1px solid black;
  width: 20px;
  margin-top: 5px;
}
.line3 {
  border: 1px solid black;
  width: 20px;
  margin-top: 5px;
}
.navs {
  display: flex;
  justify-content: flex-end;
  align-items: center;
  font-weight: 700;
  font-size: 14px;
  width: 100%;
}

.navs > div {
  margin: 25px;
}
.box {
  display: flex;
}
.items {
  display: flex;
  align-items: center;
}
.items > div {
  margin-right: 20px;
}

.redbutton {
  color: white;
  border-radius: 5px;
  background-color: #f84646;
  padding: 10px;
  width: 77px;
  text-align: center;
}
.contents {
  margin-top: 10%;
  font-size: 10px;
  margin-left: 20px;
  margin-right: 20px;
}
.title {
  width: 100%;
  font-size: 40px;
  text-align: center;
}
.content {
  margin-top: 20px;
  text-align: center;
  font-size: 12px;
}
.mail {
  display: inline-block;
  width: 100%;
  background: #ffff;
  border-radius: 8px;
  margin-top: 40px;
  margin-bottom: 20px;
}
.mail > div {
  padding: 6px;
}
.mail input {
  outline: none;
  border: none;
  font-size: 14px;
  color: rgba(0, 0, 0, 0.4);
  padding: 15px;
  border-radius: 8px;
}

.mailsend {
  float: right;
  width: 66px;
  text-align: center;
  padding: 15px;
  font-size: 14px;
}
.line1 {
  stroke-dasharray: 60 207;
  stroke-width: 6;
}
.line2 {
  stroke-dasharray: 60 60;
  stroke-width: 6;
}
.line3 {
  stroke-dasharray: 60 207;
  stroke-width: 6;
}
@media (min-width: 375px) and (max-width: 1023px) {
  .items {
    display: none !important;
  }
  .hamburger {
    visibility: visible;
  }
  .contents1 {
    display: none !important;
  }
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .hamburger {
    display: none !important;
  }
  .contents {
    display: none !important;
  }
}
@media (min-width: 1440px) {
  .hamburger {
    display: none !important;
  }
  .mail {
    display: inline-block;
    width: 100%;
    background: #ffff;
    border-radius: 8px;
    margin-top: 40px;
    margin-bottom: 20px;
  }
  .mailsend {
    float: right;
    width: 66px;
    text-align: center;
    padding: 15px;
    font-size: 16px;
  }
  .contents {
    display: none !important;
  }
  .navs {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    font-weight: 700;
    font-size: 14px;
    width: 100%;
  }

  .navs > div {
    margin: 25px;
    margin-right: 60px;
  }
  .box {
    display: flex;
  }
  .items {
    display: flex;
    align-items: center;
  }
  .items > div {
    margin-right: 20px;
  }
  .mailsend {
    float: right;
    width: 66px;
    text-align: center;
    padding: 15px;
    font-size: 14px;
  }
}
</style>
