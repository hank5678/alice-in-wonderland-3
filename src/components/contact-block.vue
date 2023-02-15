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
.icon__first {
  position: relative;
  z-index: 1;
}
.icon__first > img {
  width: 90px;
  height: 90px;
}

.icon__sec {
  position: absolute;
  left: 41px;
  top: 5px;
  z-index: 0;
}

.icon__sec > img {
  width: 45px;
  height: 45px;
}
.title {
  height: 32px;
  font-size: 36px;
  font-weight: 800;
  text-align: center;
  margin-bottom: 12px;
  line-height: 0.89;
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
.contactbtn {
  width: 34%;
  margin: 20px auto;
}
</style>
