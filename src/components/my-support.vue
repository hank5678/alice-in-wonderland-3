<template>
  <div class="support__item" v-for="(item, index) of items" :key="item">
    <div class="support">
      <div class="support__title">{{ item.title }}</div>
      <div class="support__icon" v-if="items.length - 1 != index">
        <img :src="item.icon" alt="" />
      </div>
    </div>
  </div>
</template>
<script setup>
import icon1 from "@/assets/icons/CaretCircleDoubleRight.png"

import { ref } from "vue"

let items = ref([
  { title: "Yazılım Kalitesini Arttırıyoruz", icon: icon1 },
  {
    title: "Olası Hataları Önceden Belirliyoruz",
    icon: icon1
  },
  { title: "Oluşabilecek Riskleri Önlüyoruz", icon: icon1 },
  {
    title: "Zaman ve Maliyetten Tasarruf Sağlıyoruz",
    icon: icon1
  }
])
</script>

<style scoped>
.support__item {
  margin-top: 44.5px;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .support__item {
    display: inline-block;
    width: 25%;
  }
}

@media (min-width: 1440px) {
  .support__item {
    display: inline-block;
    width: 25%;
  }
}

.support {
  width: 183px;
  margin: 0 auto;
  text-align: center;
  color: #fff;
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .support {
    display: flex;
    align-items: center;
  }
}

@media (min-width: 1440px) {
  .support {
    display: flex;
    align-items: center;
  }
}

.support__title {
  font-size: 18px;
  font-weight: bold;
  text-align: center;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .support__title {
    display: flex;
    font-size: 12px;
    align-items: center;
    margin-right: 10px;
    text-align: left;
  }
}
@media (min-width: 1440px) {
  .support__title {
    display: flex;
    font-size: 12px;
    align-items: center;
    margin-right: 10px;
    text-align: left;
  }
}

.support__icon {
  margin-top: 27px;
}
.support__icon > img {
  max-width: 30px;
  transform: rotate(90deg);
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .support__icon > img {
    transform: rotate(0deg);
    max-width: 24px;
    align-items: center;
  }
}

@media (min-width: 1440px) {
  .support__icon > img {
    transform: rotate(0deg);
    max-width: 24px;
    align-items: center;
  }
}
</style>
