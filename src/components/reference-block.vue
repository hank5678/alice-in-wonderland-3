<template>
  <div class="contaniner">
    <div class="title">Referanslarımız</div>
    <div class="content">Bize güvenen ve beraber çalıştığımız iş ortaklarımız</div>
    <div class="referitem"><MyReferitem></MyReferitem></div>
  </div>
</template>
<script setup>
import MyReferitem from "./my-referitem.vue"
</script>

<style scoped>
.contaniner {
  background-color: #f4f5f7;
  padding-bottom: 20px;
}
.title {
  width: 335px;
  text-align: center;
  margin: 0 auto;
  font-size: 36px;
  font-weight: bold;
  padding-top: 40px;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .title {
    width: 693px;
    font-size: 48px;
    font-weight: 800;
    line-height: 1.33;
    color: #18191f;
  }
}
@media (min-width: 1440px) {
  .title {
    width: 693px;

    font-size: 48px;
    font-weight: 800;
    line-height: 1.33;
    color: #18191f;
  }
}
.content {
  width: 333px;
  height: 32px;
  font-size: 14px;
  font-weight: 500;
  text-align: center;
  margin: 0 auto;
  margin-top: 14px;
  margin-bottom: 40px;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .content {
    font-size: 18px;
    width: 693px;
    line-height: 1.78;
    color: #18191f;
    margin-bottom: 48px;
  }
}
@media (min-width: 1440px) {
  .content {
    font-size: 18px;
    width: 693px;
    line-height: 1.78;
    color: #18191f;
    margin-bottom: 48px;
  }
}
</style>
