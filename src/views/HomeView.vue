<template>
  <div class="home">
    <HeaderComp></HeaderComp>
    <StageTeaserComp></StageTeaserComp>
  </div>
</template>

<script>
// @ is an alias to /src
import HeaderComp from '@/components/Header.vue'
import StageTeaserComp from '@/components/StageTeaser.vue'

export default {
  name: 'HomeView',
  components: {
    HeaderComp,
    StageTeaserComp
  }
}
</script>
<style>
.home{
  position: relative
}
</style>
