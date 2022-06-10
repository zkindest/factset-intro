<script lang="ts">
import HeaderComp from './components/HeaderComp.vue';
import FooterComp from './components/FooterComp.vue';
export default {
  components: { HeaderComp, FooterComp },
};
</script>

<template>
  <div>
    <HeaderComp />
    <router-view></router-view>
    <FooterComp />
  </div>
</template>

<style>
@import url('@/assets/css/base.css');
</style>
