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
.button--readmore {
  width: 100%;
  height: 48px;
  font-size: 14px;
  line-height: 1.71;
  font-weight: 600;
}
.button--contact {
  width: 124px;
  height: 42px;
  font-size: 16px;
  font-weight: 600;
  line-height: 1.25;
}

@media (max-width: 1023px) {
  .button--mailsend {
    width: 90.8px;
    height: 50px;
    font-size: 14px;
  }
  .button--readmore {
    width: 100%;
    height: 48px;
  }
}

@media (min-width: 1024px) and (max-width: 1439px) {
  .button--mailsend {
    width: 114.3px;
    height: 61px;
    font-size: 16px;
  }
  .button--readmore {
    width: 160px;
    height: 48px;
  }
  .button--contact {
    width: 204px;
    margin: 0 auto;
    height: 70px;
    font-size: 24px;
    line-height: 0.83;
  }
}

@media (min-width: 1440px) {
  .button--mailsend {
    width: 136px;
    height: 61px;
    font-size: 16px;
  }
  .button--readmore {
    width: 160px;
    height: 48px;
  }
  .button--contact {
    width: 204px;
    margin: 0 auto;
    height: 70px;
    font-size: 24px;
    line-height: 0.83;
  }
}
</style>
