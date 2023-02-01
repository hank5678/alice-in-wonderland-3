<template>
  <div class="nav">
    <div class="hamburger">
      <div class="hamburger__line"></div>
      <div class="hamburger__line"></div>
      <div class="hamburger__line"></div>
    </div>

    <!-- <div class="box"> -->
    <div class="list">
      <div class="list__item">Çözüm ve Hizmetler</div>
      <div class="list__item">Ürünler</div>
      <div class="list__item">Teknolojiler</div>
      <div class="list__item">İnsan Kaynakları</div>
      <div class="list__item">Kurumsal</div>
    </div>
    <!-- </div> -->

    <my-button>İletişim</my-button>
  </div>
</template>

<script setup>
import MyButton from "./my-button.vue"
</script>

<style scoped>
/* nav */
.nav {
  display: flex;
  align-items: center;
}

@media (max-width: 1023px) {
  .nav {
    padding: 35px 20px 0 20px;
    margin-bottom: 62px;
    justify-content: space-between;
  }
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .nav {
    padding: 35px 40px 0 40px;
    margin-bottom: 86px;
    justify-content: flex-end;
  }
}
@media (min-width: 1440px) {
  .nav {
    padding: 35px 122px 0 122px;
    margin-bottom: 125px;
    justify-content: flex-end;
  }
}

/* hamburger */
@media (max-width: 1023px) {
  .hamburger__line {
    border: 1px solid black;
    width: 20px;
  }
  .hamburger__line:nth-child(2),
  .hamburger__line:nth-child(3) {
    margin-top: 5px;
  }
}
@media (min-width: 1024px) and (max-width: 1439px) {
  .hamburger {
    display: none;
  }
}
@media (min-width: 1440px) {
  .hamburger {
    display: none;
  }
}

/* list */
.list {
  display: flex;
  align-items: center;
}
.list__item {
  margin-right: 40px;
}
.list__item:hover {
  cursor: pointer;
  color: #0f29e8;
}

@media (max-width: 1023px) {
  .list {
    display: none;
  }
}
</style>
