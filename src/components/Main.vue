<template>
  <div>
    <MainHero></MainHero>
    <InfoMain></InfoMain>
    <HelpMain></HelpMain>
    <CourseMain></CourseMain>
    <NetworkMain></NetworkMain>
  </div>
</template>

<script>
import CourseMain from "./CourseMain.vue";
import HelpMain from "./HelpMain.vue";
import InfoMain from "./InfoMain.vue";
import MainHero from "./MainHero.vue";
import NetworkMain from "./NetworkMain.vue";
export default {
  components: { MainHero, InfoMain, HelpMain, CourseMain, NetworkMain },
  name: "Main",
};
</script>

<style>
</style>