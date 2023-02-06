<template>
  <div class="item" v-for="item of items" :key="item.id">
    <div class="item__icon">
      <img :src="item.icon" alt="" />
    </div>
    <div class="item__title">
      {{ item.title }}
    </div>
    <div class="item__content">
      {{ item.content }}
    </div>
  </div>
</template>
<script setup>
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
  }
}
@media (min-width: 1440px) {
  .item {
    width: 33%;
  }
}
</style>
