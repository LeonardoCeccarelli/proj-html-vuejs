<template>
  <div>
    <div class="info_section">
      <!-- Sezione titolo -->
      <div class="info_section_title">
        <p class="m_bottom head_title">Let's Dream Big Together</p>
        <h3>
          We are pioneers of a digital approach, using leading-edge technology
          to simplify procedures ad apply executive coaching in the new age of
          digitalization.
        </h3>
      </div>
      <!-- Contenitore card -->
      <ul class="info_section_card_container">
        <!-- Singola card -->
        <li
          v-for="(item, i) in listInfoCard"
          :key="i"
          class="info_section_card"
        >
          <div class="icon_container">
            <i :class="item.iconPath"></i>
          </div>
          <div class="text_container">
            <h3 class="m_bottom">{{ item.title }}</h3>
            <p>{{ item.text }}</p>
          </div>
        </li>
      </ul>
      <!-- Sezione bottoni -->
      <div class="info_section_btn_container">
        <button class="btun btun_white_primary" type="button">
          Learn more
        </button>
        <button class="btun btun_primary" type="button">
          Get started today
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "InfoMain",
  data() {
    return {
      listInfoCard: [
        {
          iconPath: "fa fa-laptop",
          title: "One to One",
          text: "Getting the necessary claily about the current state to help you improve your game.",
        },
        {
          iconPath: "fa fa-map-marker",
          title: "Anywhere",
          text: "Access to valuable and portable program which allow you to setup and live anywhere you want.",
        },
        {
          iconPath: "fa fa-clock-o",
          title: "On Time",
          text: "Punctuality is our top priority beacuse it's an essential criteria to access a program quality.",
        },
        {
          iconPath: "fa fa-users",
          title: "Online Courses",
          text: "Online buisness coaching now offers you a very powerfull way to empower your buisness to succes.",
        },
        {
          iconPath: "fa fa-line-chart",
          title: "Consulting",
          text: "You will get a clear sense of direcion for your buisness, thorough assessment and faster result",
        },
        {
          iconPath: "fa fa-cog",
          title: "Self Development",
          text: "Buisness coaching often keep your focus and develop you both in a professional and personal way",
        },
      ],
    };
  },
};
</script>

<style>
</style>