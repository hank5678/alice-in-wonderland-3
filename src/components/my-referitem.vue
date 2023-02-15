<template>
  <div class="container">
    <div class="item">
      <div class="item__icon">
        <img :src="icon1" alt="" />
      </div>
    </div>
    <div class="item">
      <div class="item__icon">
        <img :src="icon2" alt="" />
      </div>

      <div class="item__icon">
        <img :src="icon3" alt="" />
      </div>
    </div>
    <div class="item">
      <div class="item__icon">
        <img :src="icon4" alt="" />
      </div>
      <div class="item__icon">
        <img :src="icon5" alt="" />
      </div>
      <div class="item__icon">
        <img :src="icon6" alt="" />
      </div>
    </div>
    <div class="item">
      <div class="item__icon">
        <img :src="icon7" alt="" />
      </div>
      <div class="item__icon">
        <img :src="icon8" alt="" />
      </div>
    </div>
    <div class="item">
      <div class="item__icon">
        <img :src="icon9" alt="" />
      </div>
    </div>
  </div>
</template>
<script setup>
import icon1 from "@/assets/icons/image 6.png"
import icon2 from "@/assets/icons/image 5.png"
import icon3 from "@/assets/icons/BookMyShow Logo.png"
import icon4 from "@/assets/icons/image 2.png"
import icon5 from "@/assets/icons/image 3.png"
import icon6 from "@/assets/icons/Frame 4.png"
import icon7 from "@/assets/icons/image 4.png"
import icon8 from "@/assets/icons/Group.png"
import icon9 from "@/assets/icons/Amazon Logo.png"
</script>
<style scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.item__icon {
  background-color: #fff;
  margin-bottom: 24px;
  padding-top: 20px;
  border-radius: 16px;
  width: 170px;
  height: 96px;
  text-align: center;
}

.item:nth-child(4),
:nth-child(5) {
  display: none;
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .item {
    border-radius: 16px;
    margin: 120px 24px 120px 0px;
    text-align: center;
    padding: 30px 23px 29px 24px;
  }
  .item__icon {
    background: #fff;
    border-radius: 16px;
    margin: 0 0 24px;
    padding: 18px 24px 17px;
  }
}
</style>
