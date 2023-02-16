<template>
  <div class="container">
    <div class="article">
      <div class="article__image"><img :src="image1" alt="" /></div>
      <div class="article__block">
        <div class="article__title">Kalite ve Süreç Yönetimi</div>
        <div class="article__content">
          Deneyimli kadromuz; birçok farklı sektörden deneyimli, PMP® sertifikasına sahip, uzman proje yöneticilerinden oluşmaktadır. Projelerinizin yönetimine
          destek olmak, zayıf olduğunu düşündüğünüz alanları güçlendirmek, uluslararası geçerliliği olan PMI® metodolojisini şirketinizde uygulamak ve
          geliştirmek için yanınızdayız.
        </div>
        <div class="article__readmore"><my-button modifier="readmore">Keşfet</my-button></div>
      </div>
    </div>
    <div class="article">
      <div class="article__image"><img :src="image2" alt="" /></div>
      <div class="article__block">
        <div class="article__title">Kalite ve Süreç Yönetimi</div>
        <div class="article__content">
          Deneyimli kadromuz; birçok farklı sektörden deneyimli, PMP® sertifikasına sahip, uzman proje yöneticilerinden oluşmaktadır. Projelerinizin yönetimine
          destek olmak, zayıf olduğunu düşündüğünüz alanları güçlendirmek, uluslararası geçerliliği olan PMI® metodolojisini şirketinizde uygulamak ve
          geliştirmek için yanınızdayız.
        </div>
        <div class="article__readmore"><my-button modifier="readmore">Keşfet</my-button></div>
      </div>
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
  margin-bottom: 140px;
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .article {
    width: 80%;
    margin: 120px auto;
    display: flex;
    justify-content: space-around;
  }
}
@media (min-width: 1440px) {
  .article {
    width: 80%;
    margin: 0 auto;
    display: flex;
    justify-content: space-around;
    align-items: center;
  }
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .article:nth-child(1) {
    flex-direction: row-reverse;
  }
}
@media (min-width: 1440px) {
  .article:nth-child(1) {
    flex-direction: row-reverse;
  }
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .article__block {
    width: 424px;
    height: 404px;
  }
}
@media (min-width: 1440px) {
  .article__block {
    width: 504px;
    height: 480px;
  }
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .article__image {
    width: 424px;
    height: 404px;
  }
}
@media (min-width: 1440px) {
  .article__image {
    width: 504px;
    height: 480px;
    text-align: center;
    margin-top: 90px;
  }
}

.article__image > img {
  width: 335px;
  height: 312px;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .article__image > img {
    width: 424px;
    height: 404px;
  }
}
@media (min-width: 1440px) {
  .article__image > img {
    width: 504px;
    height: 480px;
  }
}
.article__title {
  width: 335px;
  height: 83px;
  font-size: 36px;
  font-weight: bold;
  text-align: center;
  margin-top: 30px;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .article__title {
    width: 515px;
    height: 119px;
    font-size: 58px;
    text-align: left;
    line-height: 1.03;
    color: #2e2e2e;
    margin-top: 0px;
  }
}
@media (min-width: 1440px) {
  .article__title {
    width: 608px;
    height: 152px;
    font-size: 58px;
    text-align: left;
    line-height: 1.03;
    color: #2e2e2e;
    margin-top: 40px;
  }
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
@media (min-width: 1024px) and (max-width: 1439px) {
  .article__content {
    width: 428px;
    height: 171px;
    text-align: left;
    color: #808080;
  }
}
@media (min-width: 1440px) {
  .article__content {
    width: 428px;
    height: 171px;
    text-align: left;
    color: #808080;
  }
}
.article__readmore {
  margin-bottom: 60px;
}
</style>
