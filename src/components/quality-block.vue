<template>
  <div class="container">
    <div class="title">Kalite ve Süreç Yönetimi</div>
    <div class="content">
      Müşterilerimizin yüksek kalite seviyelerini koruyabilmeleri için farklı sektörlerde tecrübe kazanmış uzman kadrolarımızla Proje Yönetimi, İş Analizi ve
      Test Yönetimi hizmetleri sunmaktayız.
    </div>
    <div class="manage">
      <div class="item" v-for="item of items" :key="item.id">
        <myItem :item__icon="item.icon" :item__title="item.title" :item__content="item.content"></myItem>
      </div>
    </div>
  </div>
</template>
<script setup>
import myItem from "./my-item.vue"
import { ref } from "vue"
import icon1 from "@/assets/icons/group 27.png"
import icon2 from "@/assets/icons/group 29.png"
import icon3 from "@/assets/icons/group 32.png"
import icon4 from "@/assets/icons/group 31.png"
import icon5 from "@/assets/icons/group 33.png"
import icon6 from "@/assets/icons/group 30.png"
let items = ref([
  {
    icon: icon1,
    title: "Döküman Analizi",
    content: "Ante vulputate ut at accumsan et. Feugiat at tempus, est senectus amet, elementum."
  },
  {
    icon: icon2,
    title: "Kabul ve Değerlendirme",
    content: "Ante vulputate ut at accumsan et. Feugiat at tempus, est senectus amet, elementum."
  },
  {
    icon: icon3,
    title: "Kabul ve Değerlendirme",
    content: "Ante vulputate ut at accumsan et. Feugiat at tempus, est senectus amet, elementum."
  },
  {
    icon: icon4,
    title: "Kabul ve Değerlendirme",
    content: "Ante vulputate ut at accumsan et. Feugiat at tempus, est senectus amet, elementum."
  },
  {
    icon: icon5,
    title: "Kabul ve Değerlendirme",
    content: "Ante vulputate ut at accumsan et. Feugiat at tempus, est senectus amet, elementum."
  },
  {
    icon: icon6,
    title: "Kabul ve Değerlendirme",
    content: "Ante vulputate ut at accumsan et. Feugiat at tempus, est senectus amet, elementum."
  }
])
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

.item__icon {
  text-align: center;
}
.item__title {
  width: 284px;
  height: 31px;
  margin: 0 auto;
  font-size: 24px;
  font-weight: 800;
  color: #000;
  text-align: center;
}
.item__content {
  width: 298px;
  height: 83px;
  margin: 0 auto;
  margin-top: 10px;
  font-size: 18px;
  line-height: 1.56;
  text-align: center;
  color: #000;
}
.item {
  height: 212px;
  flex-grow: 0;
  margin-top: 40px;
  margin-bottom: 80px;
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .item {
    width: 50%;
    text-align: center;
  }
}
@media (min-width: 1440px) {
  .item {
    width: 33%;
    text-align: center;
  }
}
</style>
