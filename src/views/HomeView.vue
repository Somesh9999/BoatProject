<template>
  <div class="home">
    <HeaderComp></HeaderComp>
    <StageTeaserComp></StageTeaserComp>
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

export default {
  name: 'HomeView',
  components: {
    HeaderComp,
    StageTeaserComp,
    ProductListComp,
    FooterComp
  }
}
</script>
<style>
</style>
