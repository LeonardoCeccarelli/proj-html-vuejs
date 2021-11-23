<template>
  <div>
    <MainHero></MainHero>
    <InfoMain></InfoMain>
    <HelpMain></HelpMain>
    <CourseMain></CourseMain>
    <NetworkMain></NetworkMain>
    <EventMain></EventMain>
  </div>
</template>

<script>
import CourseMain from "./CourseMain.vue";
import EventMain from "./EventMain.vue";
import HelpMain from "./HelpMain.vue";
import InfoMain from "./InfoMain.vue";
import MainHero from "./MainHero.vue";
import NetworkMain from "./NetworkMain.vue";
export default {
  components: {
    MainHero,
    InfoMain,
    HelpMain,
    CourseMain,
    NetworkMain,
    EventMain,
  },
  name: "Main",
};
</script>

<style>
</style>