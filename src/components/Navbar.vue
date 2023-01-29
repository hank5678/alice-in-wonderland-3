<template>
  <div class="container">
    <div class="navs">
      <div class="mobile">
        <div class="hamburger">
          <div class="line line1"></div>
          <div class="line line2"></div>
          <div class="line line3"></div>
        </div>
      </div>
      <div class="desktop">
        <div class="box">
          <div class="items">
            <div>Çözüm ve Hizmetler</div>
            <div>Ürünler</div>
            <div>Teknolojiler</div>
            <div>İnsan Kaynakları</div>
            <div>Kurumsal</div>
          </div>
        </div>
      </div>
      <div class="redbutton">İletişim</div>
    </div>

    <div class="contents mobile">
      <div class="title">Bilgi <br />Teknolojilerinde <br />23 Yıllık Tecrübe</div>
      <div class="content">
        Müşterilerimizin yüksek kalite seviyelerini koruyabilmeleri için farklı sektörlerde tecrübe kazanmış uzman<br />
        kadrolarımızla Proje Yönetimi, İş Analizi ve Test Yönetimi hizmetleri sunmaktayız.
      </div>
    </div>
    <div class="contents desktop">
      <div class="title">Bilgi Teknolojilerinde <br />23 Yıllık Tecrübe</div>
      <div class="content">
        Müşterilerimizin yüksek kalite seviyelerini koruyabilmeleri için farklı <br />sektörlerde tecrübe kazanmış uzman kadrolarımızla Proje Yönetimi, İş<br />
        Analizi ve Test Yönetimi hizmetleri sunmaktayız.
      </div>
    </div>

    <div>
      <div class="mail">
        <div>
          <input type="text" placeholder="Mail bültenimize kayıt ol" />
        </div>
        <div class="redbutton mailsend">Kayıt Ol</div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.container {
  background-image: radial-gradient(circle at 141% 78%, #fff, rgba(255, 255, 255, 0) 107%), url("@/assets/images/rectangle-1.jpg");
  background-size: cover;
  height: 100vh;
  background-position: right 35% bottom 45%;
  width: 100%;
}
.navs {
  display: flex;
  justify-content: space-between;
  padding: 20px;
  align-items: center;
}

.redbutton {
  background-color: #f84646;
  color: #fff;
  padding: 10px;
  border-radius: 5px;
  font-size: 14px;
  width: 91px;
  text-align: center;
}
.items > div:hover {
  cursor: pointer;
  color: #0f29e8;
}
.redbutton:hover {
  cursor: pointer;
  background-color: #0f29e8;
  transition: 0.8s;
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
.mailsend {
  width: 90.8px !important;
  height: 30px !important;
  padding-top: 15px;
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

@media (min-width: 375px) and (max-width: 1023px) {
  .mobile {
    display: block !important;
  }
  .desktop {
    display: none !important;
  }
  .items {
    display: none !important;
  }
  .hamburger {
    visibility: visible;
  }
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .mobile {
    display: none !important;
  }
  .desktop {
    display: block !important;
  }
  .container {
    background-image: url("@/assets/images/rectangle-1.jpg");
    height: 100vh;
    background-position: 0px 0px;
  }
  .navs {
    display: flex;
  }
  .hamburger {
    display: none !important;
  }
  .navs {
    justify-content: flex-end;
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
    margin-top: 93px;
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
  .mobile {
    display: none !important;
  }
  .desktop {
    display: block !important;
  }
  .container {
    background-image: url("@/assets/images/rectangle-1.jpg");

    background-position: 0px 0px;
  }

  .hamburger {
    display: none !important;
  }
  .navs {
    justify-content: flex-end;
  }

  .box {
    display: flex;
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
    margin-top: 93px;
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
