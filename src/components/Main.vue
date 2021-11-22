<template>
  <div>
    <MainHero></MainHero>
    <InfoMain><InfoMain>
  </div>
</template>

<script>
import InfoMain from "./InfoMain.vue";
import MainHero from "./MainHero.vue";
export default {
  components: { MainHero, InfoMain },
  name: "Main",
};
</script>

<style>
</style>