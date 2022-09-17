<template>
  <div class="home">
    <HeaderComp></HeaderComp>
    <StageTeaserComp></StageTeaserComp>
    <StageButtonComp></StageButtonComp>
    <ProductListComp></ProductListComp>
    <FooterComp></FooterComp>
  </div>
</template>

<script>
// @ is an alias to /src
import HeaderComp from '@/components/Header.vue'
import StageTeaserComp from '@/components/StageTeaser.vue'
import ProductListComp from '@/components/Products.vue'
import FooterComp from '@/components/Footer.vue'
import StageButtonComp from '@/components/StageButtons.vue'

export default {
  name: 'HomeView',
  components: {
    HeaderComp,
    StageTeaserComp,
    ProductListComp,
    FooterComp,
    StageButtonComp
  }
}
</script>
<style>
@media (max-width: 600px) {
    .home{
      font-size: 12px;
    }
}
</style>
