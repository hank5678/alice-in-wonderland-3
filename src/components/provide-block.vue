<template>
  <div class="container">
    <div class="title">Test Yönetimiyle Neler Sağlıyoruz?</div>
    <div class="content">IoT Destekli Çözümler</div>
    <div class="support">
      <mySupport />
    </div>
  </div>
</template>
<script setup>
import mySupport from "./my-support.vue"
</script>

<style scoped>
.container {
  background-color: #f84646;
  padding: 21px;
}

.content {
  margin: 0 auto;
  width: 190px;
  height: 32px;
  font-size: 14px;
  font-size: 14px;
  text-align: center;
  color: #fff;
  margin-top: 9px;
  line-height: 2.29;
}

.title {
  width: 335px;
  height: 94px;
  font-size: 36px;
  margin: 0 auto;
  text-align: center;
  color: #fff;
  font-weight: 800;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .title {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
}
@media (min-width: 1440px) {
  .title {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
}
.support {
  margin-top: 55px;
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .support {
    width: 80%;
    margin: 0 auto;
    justify-content: space-evenly;
  }
}
@media (min-width: 1440px) {
  .support {
    width: 80%;
    margin: 0 auto;
    justify-content: space-evenly;
  }
}
</style>
