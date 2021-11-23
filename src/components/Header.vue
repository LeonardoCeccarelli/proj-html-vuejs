<template>
  <div>
    <nav>
      <!-- Sezione logo -->
      <div class="nav_logo">
        <div class="logo_container">
          <img src="@/assets/dark-logo.png" alt="text logo" />
        </div>
      </div>
      <!-- Sezione lista link -->
      <div class="nav_link">
        <ul>
          <!-- Singolo link -->
          <li tabindex="0" v-for="(link, i) in linkNavList" :key="i">
            <a>{{ link.text }}</a>
            <i class="fa fa-angle-down"></i>
            <div class="dropdown_menu">
              <a :href="link.url">Link DropDown Menu</a>
              <a :href="link.url">Altro Link</a>
            </div>
          </li>
        </ul>
      </div>
      <!-- Sezione settaggi -->
      <div class="nav_search">
        <div class="nav_search_language">
          <!-- Logo bandiera -->
          <div class="image_container">
            <img src="@/assets/en.png" alt="flag logo" />
          </div>
          <!-- Testo lingua -->
          <div class="language_container">
            <a href="#">English</a>
            <i class="fa fa-angle-down"></i>
          </div>
          <!-- Icona profilo -->
          <div class="user_icon_container">
            <i class="fa fa-user-circle-o"></i>
          </div>
        </div>
        <div class="nav_search_input">
          <input type="text" placeholder="Search..." />
          <i class="fa fa-search"></i>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      linkNavList: [
        {
          text: "home",
          url: "#home",
        },
        {
          text: "pages",
          url: "#pages",
        },
        {
          text: "Courses",
          url: "#Courses",
        },
        {
          text: "Features",
          url: "#Features",
        },
        {
          text: "blog",
          url: "#blog",
        },
        {
          text: "shop",
          url: "#shop",
        },
      ],
    };
  },
};
</script>

<style>
</style>