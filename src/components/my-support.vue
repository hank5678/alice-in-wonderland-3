<template>
  <div class="support">
    <template v-for="(item, index) of items" :key="index">
      <div class="support__title">{{ item.title }}</div>
      <img class="support__icon" :src="item.icon" alt="" v-if="items.length - 1 != index" />
    </template>
  </div>
</template>
<script setup>
import icon1 from "@/assets/icons/CaretCircleDoubleRight.png"

import { ref } from "vue"

let items = ref([
  { title: "Yazılım Kalitesini\nArttırıyoruz", icon: icon1 },
  {
    title: "Olası Hataları Önceden\nBelirliyoruz",
    icon: icon1
  },
  { title: "Oluşabilecek Riskleri\nÖnlüyoruz", icon: icon1 },
  {
    title: "Zaman ve Maliyette\nTasarruf Sağlıyoruz",
    icon: icon1
  }
])
</script>

<style scoped>
.support {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin: 55px auto 0 auto;
}

@media (max-width: 1023px) {
  .support {
    flex-direction: column;
    height: 500px;
  }
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .support {
    max-width: 906px;
  }
}
@media (min-width: 1440px) {
  .support {
    max-width: 1088px;
  }
}

.support__title {
  white-space: pre-line;
  color: #ffffff;
  font-weight: bold;
}
@media (max-width: 1023px) {
  .support__title {
    font-size: 18px;
  }
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .support__title {
    font-size: 14px;
  }
}
@media (min-width: 1440px) {
  .support__title {
    font-size: 18px;
  }
}

@media (max-width: 1023px) {
  .support__icon {
    transform: rotate(90deg);
  }
}
</style>
