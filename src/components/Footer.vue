<template>
  <div>
    <div class="footer_container">
      <div class="footer_content">
        <div class="footer_address_container">
          <p class="footer_title m_bottom">Address</p>
          <p class="footer_subtitle m_bottom">
            382 NE 191st St # 87394 Miami, FL 33179-3899
          </p>
          <p class="footer_subtitle m_bottom">
            +1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)
          </p>
          <p class="footer_subtitle footer_last_item">support@maxcoach.com</p>
          <div class="icon_footer_container">
            <i class="fa fa-facebook-square"></i>
            <i class="fa fa-twitter"></i>
            <i class="fa fa-instagram"></i>
            <i class="fa fa-linkedin-square"></i>
          </div>
        </div>
        <div class="footer_link_container">
          <div class="footer_link_explore">
            <p class="footer_title m_bottom">Explore</p>
            <ul class="footer_link_sx">
              <li v-for="(link, i) in listLinkExplore" :key="'explore_' + i">
                <a class="footer_subtitle" :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="footer_link_information">
            <p class="footer_title m_bottom">Information</p>
            <ul>
              <li v-for="(link, i) in listLinkInformation" :key="i">
                <a class="footer_subtitle" :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="footer_copyright_container">
          <p class="footer_subtitle">© 2020 Maxcoach. All Right Reserved</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      listLinkExplore: [
        {
          text: "Start here",
          url: "#Start_here",
        },
        {
          text: "Blog",
          url: "Blog",
        },
        {
          text: "About us",
          url: "#About_us",
        },
        {
          text: "Succes day",
          url: "#Succes_day",
        },
        {
          text: "Courses",
          url: "#Courses",
        },
        {
          text: "Contact us",
          url: "#Contact_us",
        },
      ],
      listLinkInformation: [
        {
          text: "Membership",
          url: "#Membership",
        },
        {
          text: "Purchase guide",
          url: "#Purchase_guide",
        },
        {
          text: "Privacy policy",
          url: "#Privacy_policy",
        },
        {
          text: "Terms of service",
          url: "#Terms_of_service",
        },
      ],
    };
  },
};
</script>

<style>
</style>