<template>
  <div class="item__icon">
    <img :src="props.item__icon" alt="" />
  </div>

  <div class="item__title">
    {{ props.item__title }}
  </div>

  <div class="item__content">
    {{ props.item__content }}
  </div>
</template>
<script setup>
const props = defineProps({
  item__icon: String,
  item__title: String,
  item__content: String
})
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
