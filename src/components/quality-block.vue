<template>
  <div class="container">
    <div class="title">Kalite ve Süreç Yönetimi</div>
    <div class="content">
      Müşterilerimizin yüksek kalite seviyelerini koruyabilmeleri için farklı sektörlerde tecrübe kazanmış uzman kadrolarımızla Proje Yönetimi, İş Analizi ve
      Test Yönetimi hizmetleri sunmaktayız.
    </div>
    <div class="manage">
      <myItem></myItem>
    </div>
  </div>
</template>
<script setup>
import myItem from "./my-item.vue"
</script>
<style scoped>
.container {
  padding: 21px;
  width: 375px;
  margin: 0 auto;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .container {
    padding: 86px;
    width: 852px;
  }
}
@media (min-width: 1440px) {
  .container {
    width: 100%;
  }
}
.title {
  width: 286px;
  margin: 0 auto;
  margin-top: 60px;
  height: 31px;
  font-size: 24px;
  font-weight: 800;
  text-align: center;
  color: #000;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .title {
    width: 428px;
    height: 56px;
    font-size: 36px;
  }
}
@media (min-width: 1440px) {
  .title {
    width: 428px;
    height: 56px;
    font-size: 36px;
  }
}

.content {
  width: 334px;
  margin: 0 auto;
  font-size: 12px;
  text-align: center;
  margin-bottom: 80px;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .content {
    width: 852px;
    height: 109px;
    font-size: 24px;
    line-height: 1.65;
  }
}
@media (min-width: 1440px) {
  .content {
    width: 994px;
    height: 109px;
    font-size: 24px;
    line-height: 1.65;
  }
}
.manage {
  display: block;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .manage {
    display: flex;
    flex-wrap: wrap;
  }
}
@media (min-width: 1440px) {
  .manage {
    display: flex;
    flex-wrap: wrap;
  }
}
</style>
