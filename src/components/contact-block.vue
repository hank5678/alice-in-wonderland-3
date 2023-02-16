<template>
  <div class="container">
    <div class="icon">
      <div class="icon__first">
        <img :src="icon1" alt="" />
      </div>
      <div class="icon__sec">
        <img :src="icon2" alt="" />
      </div>
    </div>
    <div class="title">Bize Ulaşın</div>
    <div class="content">Çözüm, hizmet ve ürünlerimiz hakkında detaylı bilgi için bizimle irtibata geçin.</div>
    <div class="contactbtn"><MyButton modifier="contact">Bize Ulaşın</MyButton></div>
  </div>
</template>
<script setup>
import MyButton from "./my-button.vue"
import icon1 from "@/assets/icons/Users.png"
import icon2 from "@/assets/icons/Ellipse 5.png"
</script>
<style scoped>
.container {
  padding: 20px;
  margin-bottom: 82px;
}
.icon {
  position: relative;
  margin: 0 auto;
  margin-bottom: 20px;
  width: 90px;
  height: 90px;
  margin-top: 90px;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .icon {
    width: 120px;
    height: 120px;
  }
}
@media (min-width: 1440px) {
  .icon {
    width: 120px;
    height: 120px;
  }
}

.icon__first {
  position: relative;
  z-index: 1;
}
.icon__first > img {
  width: 90px;
  height: 90px;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .icon__first > img {
    width: 120px;
    height: 120px;
  }
}
@media (min-width: 1440px) {
  .icon__first > img {
    width: 120px;
    height: 120px;
  }
}

.icon__sec {
  position: absolute;
  left: 41px;
  top: 5px;
  z-index: 0;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .icon__sec {
    left: 55px;
  }
}
@media (min-width: 1440px) {
  .icon__sec {
    left: 55px;
  }
}

.icon__sec > img {
  width: 45px;
  height: 45px;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .icon__sec > img {
    width: 61px;
    height: 61px;
  }
}

.title {
  height: 32px;
  font-size: 36px;
  font-weight: 800;
  text-align: center;
  margin-bottom: 12px;
  line-height: 0.89;
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .title {
    font-size: 48px;
    line-height: 0.67;
    margin-bottom: 20px;
  }
}
@media (min-width: 1440px) {
  .title {
    font-size: 48px;
    line-height: 0.67;
    margin-bottom: 20px;
  }
}
.content {
  width: 335px;
  height: 50px;
  font-size: 14px;
  font-weight: 500;
  line-height: 1.79;
  text-align: center;
  color: #000;
  margin: 0 auto;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .content {
    font-size: 18px;
    line-height: 1.78;
    width: 645px;
    height: 32px;
    margin-bottom: 30px;
  }
}
@media (min-width: 1440px) {
  .content {
    font-size: 18px;
    line-height: 1.78;
    width: 645px;
    height: 32px;
    margin-bottom: 30px;
  }
}
.contactbtn {
  width: 34%;
  margin: 20px auto;
}
</style>
