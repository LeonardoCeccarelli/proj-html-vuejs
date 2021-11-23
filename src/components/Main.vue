<template>
  <div>
    <MainHero></MainHero>
    <InfoMain></InfoMain>
    <HelpMain></HelpMain>
    <CourseMain></CourseMain>
    <NetworkMain></NetworkMain>
    <EventMain></EventMain>
    <ReviewMain></ReviewMain>
    <SubscribeMain></SubscribeMain>
  </div>
</template>

<script>
import CourseMain from "./CourseMain.vue";
import EventMain from "./EventMain.vue";
import HelpMain from "./HelpMain.vue";
import InfoMain from "./InfoMain.vue";
import MainHero from "./MainHero.vue";
import NetworkMain from "./NetworkMain.vue";
import ReviewMain from "./ReviewMain.vue";
import SubscribeMain from "./SubscribeMain.vue";
export default {
  components: {
    MainHero,
    InfoMain,
    HelpMain,
    CourseMain,
    NetworkMain,
    EventMain,
    ReviewMain,
    SubscribeMain,
  },
  name: "Main",
};
</script>

<style>
</style>