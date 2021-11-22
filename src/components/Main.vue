<template>
  <div>
    <MainHero></MainHero>
    <InfoMain></InfoMain>
    <HelpMain></HelpMain>
    <CourseMain></CourseMain>
  </div>
</template>

<script>
import CourseMain from "./CourseMain.vue";
import HelpMain from "./HelpMain.vue";
import InfoMain from "./InfoMain.vue";
import MainHero from "./MainHero.vue";
export default {
  components: { MainHero, InfoMain, HelpMain, CourseMain },
  name: "Main",
};
</script>

<style>
</style>