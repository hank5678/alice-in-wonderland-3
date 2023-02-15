<template>
  <div class="container">
    <div class="article">
      <div class="article__image"><img :src="image1" alt="" /></div>
      <div class="article__title">Kalite ve Süreç Yönetimi</div>
      <div class="article__content">
        Deneyimli kadromuz; birçok farklı sektörden deneyimli, PMP® sertifikasına sahip, uzman proje yöneticilerinden oluşmaktadır. Projelerinizin yönetimine
        destek olmak, zayıf olduğunu düşündüğünüz alanları güçlendirmek, uluslararası geçerliliği olan PMI® metodolojisini şirketinizde uygulamak ve geliştirmek
        için yanınızdayız.
      </div>
      <div class="article__readmore"><my-button modifier="readmore">Keşfet</my-button></div>
    </div>
    <div class="article">
      <div class="article__image"><img :src="image2" alt="" /></div>
      <div class="article__title">Kalite ve Süreç Yönetimi</div>
      <div class="article__content">
        Deneyimli kadromuz; birçok farklı sektörden deneyimli, PMP® sertifikasına sahip, uzman proje yöneticilerinden oluşmaktadır. Projelerinizin yönetimine
        destek olmak, zayıf olduğunu düşündüğünüz alanları güçlendirmek, uluslararası geçerliliği olan PMI® metodolojisini şirketinizde uygulamak ve geliştirmek
        için yanınızdayız.
      </div>
      <div class="article__readmore"><my-button modifier="readmore">Keşfet</my-button></div>
    </div>
  </div>
</template>

<script setup>
import myButton from "./my-button.vue"
import image1 from "@/assets/icons/Illustration.png"
import image2 from "@/assets/icons/Illustration_2.png"
</script>
<style scoped>
.container {
  padding: 20px;
}
.article__image {
  text-align: center;
  margin-top: 90px;
}
.article__image > img {
  width: 335px;
  height: 312px;
}
.article__title {
  width: 335px;
  height: 83px;
  font-size: 36px;
  font-weight: bold;
  text-align: center;
  margin-top: 30px;
}
.article__content {
  margin-top: 20px;
  width: 336px;
  height: 200px;
  text-align: center;
  color: #808080;
  font-size: 14px;
  line-height: 2.04;
  margin-bottom: 40px;
}
.article__readmore {
  margin-bottom: 60px;
}
</style>
