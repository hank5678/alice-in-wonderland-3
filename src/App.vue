<template>
  <div>
    <HomeBlock />
  </div>
  <div>
    <QualityBlock />
  </div>
  <div>
    <ProvideBlock />
  </div>
  <div>
    <articleBlock></articleBlock>
  </div>
  <div>
    <ReferenceBlock></ReferenceBlock>
  </div>
  <div>
    <ContactBlock></ContactBlock>
  </div>
  <div>
    <footer-block></footer-block>
  </div>
</template>

<script setup>
import HomeBlock from "./components/home-block.vue"
import ProvideBlock from "./components/provide-block.vue"
import QualityBlock from "./components/quality-block.vue"
import ReferenceBlock from "./components/reference-block.vue"
import articleBlock from "./components/article-block.vue"
import ContactBlock from "./components/contact-block.vue"
import footerBlock from "./components/footer-block.vue"
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Manrope:wght@200;300;400;500;600;700;800&display=swap");
</style>
