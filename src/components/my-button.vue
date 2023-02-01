<template>
  <div :class="['button', props.modifier && `button--${props.modifier}`]">
    <slot></slot>
  </div>
</template>

<script setup>
const props = defineProps(["modifier"])
</script>

<style scoped>
.button {
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #f84646;
  color: #fff;
  border-radius: 5px;
  font-size: 14px;
  width: 91px;
  height: 40px;
  text-align: center;
  cursor: pointer;
}
.button:hover {
  background-color: #0f29e8;
  transition: 0.8s;
}

@media (max-width: 1023px) {
  .button--mailsend {
    width: 90.8px;
    height: 50px;
    font-size: 14px;
  }
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .button--mailsend {
    width: 114.3px;
    height: 61px;
    font-size: 16px;
  }
}

@media (min-width: 1440px) {
  .button--mailsend {
    width: 136px;
    height: 61px;
    font-size: 16px;
  }
}
</style>
