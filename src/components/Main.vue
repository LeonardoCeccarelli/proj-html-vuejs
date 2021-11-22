<template>
  <div>
    <MainHero></MainHero>
    <InfoMain></InfoMain>
    <HelpMain></HelpMain>
  </div>
</template>

<script>
import HelpMain from "./HelpMain.vue";
import InfoMain from "./InfoMain.vue";
import MainHero from "./MainHero.vue";
export default {
  components: { MainHero, InfoMain, HelpMain },
  name: "Main",
};
</script>

<style>
</style>