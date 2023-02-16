<template>
  <div class="container">
    <div class="container__top">
      <div class="solution">
        <div class="solution__title">Çözüm ve Hizmetler</div>
        <div class="solution__content">
          <div class="solution__item">Yazılım Geliştirme</div>
          <div class="solution__item">Outsourcing</div>
          <div class="solution__item">Kalite ve Süreç Yönetimi</div>
          <div class="solution__item">Danışmanlık</div>
          <div class="solution__item">IoT Destekli Çözümler</div>
        </div>
      </div>
      <div class="product">
        <div class="product__title">Ürünler</div>
        <div class="product__content">
          <div class="product__item">Eğitim Yönetim Sistemi</div>
          <div class="product__item">İnsan Sermayesi Yönetim Sistemi</div>
          <div class="product__item">Müşteri İlişkileri Yönetim Sistemi</div>
          <div class="product__item">İçerik Yönetim Sistemi</div>
        </div>
      </div>
      <div class="organ">
        <div class="organ__title">Kurumsal</div>
        <div class="organ__content">
          <div class="organ__item">Hakkımızda</div>
          <div class="organ__item">Belge ve Yetkinlikler</div>
          <div class="organ__item">İş Ortakları</div>
        </div>
      </div>
      <div class="communicate">
        <div class="communicate__title">İletişim</div>
        <div class="communicate__content">
          <div class="communicate__item">İş Ortakları</div>
          <div class="communicate__item">Uzman Talep Formu</div>
        </div>
      </div>
    </div>
    <div class="container__bottom">
      <div class="icons">
        <div class="icon__item">
          <img :src="icon1" alt="" />
        </div>
        <div class="icon__item">
          <img :src="icon2" alt="" />
        </div>
        <div class="icon__item">
          <img :src="icon3" alt="" />
        </div>
        <div class="icon__item">
          <img :src="icon4" alt="" />
        </div>
        <div class="icon__item">
          <img :src="icon5" alt="" />
        </div>
      </div>
      <div class="copyright">© Copyright 2010-2021 - Can Çevik</div>
    </div>
  </div>
</template>
<script setup>
import icon1 from "@/assets/icons/MediumLogo.png"
import icon2 from "@/assets/icons/LinkedinLogo.png"
import icon3 from "@/assets/icons/TwitterLogo.png"
import icon4 from "@/assets/icons/InstagramLogo.png"
import icon5 from "@/assets/icons/FacebookLogo.png"
</script>

<style scoped>
.container {
  background: #f84646;
  padding: 20px;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .container__top {
    width: 90%;
    margin: 60px auto;
    display: flex;
    justify-content: space-between;
  }
  .container__bottom {
    width: 90%;
    margin: 0 auto;
    display: flex;
    flex-direction: row-reverse;
    justify-content: space-between;
  }
}
@media (min-width: 1440px) {
  .container__top {
    width: 80%;
    margin: 60px auto;
    display: flex;
    justify-content: space-between;
  }
  .container__bottom {
    width: 80%;
    margin: 0 auto;
    display: flex;
    flex-direction: row-reverse;
    justify-content: space-between;
  }
}
.solution {
  margin-bottom: 40px;
  width: 184px;
}

.solution__title {
  font-size: 16px;
  font-weight: bold;
  line-height: 1.5;
  color: #fff;
  margin-bottom: 24px;
}
.solution__item {
  font-size: 16px;
  line-height: 2;
  color: #e6e6e6;
  margin-bottom: 24px;
}
.product {
  width: 265px;
  margin-bottom: 40px;
}
.product__title {
  font-size: 16px;
  font-weight: bold;
  line-height: 1.5;
  color: #fff;
  margin-bottom: 24px;
}
.product__item {
  font-size: 16px;
  line-height: 2;
  color: #e6e6e6;
  margin-bottom: 24px;
}
.organ {
  width: 153px;
  margin-bottom: 40px;
}
.organ__title {
  font-size: 16px;
  font-weight: bold;
  line-height: 1.5;
  color: #fff;
  margin-bottom: 24px;
}
.organ__item {
  font-size: 16px;
  line-height: 2;
  color: #e6e6e6;
  margin-bottom: 24px;
}
.communicate {
  width: 153px;
}
.communicate__title {
  font-size: 16px;
  font-weight: bold;
  line-height: 1.5;
  color: #fff;
  margin-bottom: 24px;
}
.communicate__item {
  font-size: 16px;
  line-height: 2;
  color: #e6e6e6;
  margin-bottom: 24px;
}

.icons {
  display: flex;
  margin-bottom: 62px;
}
.icons .icon__item {
  margin-right: 20px;
}
.copyright {
  font-size: 16px;
  line-height: 2;
  color: #fff;
}
</style>
