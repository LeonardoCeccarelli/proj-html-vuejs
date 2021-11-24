<template>
  <div>
    <div class="help_section_container">
      <div class="help_section_content">
        <!-- Sezione titolo -->
        <div class="help_section_content_title">
          <p class="m_bottom head_title">Let's Dream Big Together</p>
          <h2>Explore How Can I Help You</h2>
        </div>
        <!-- Contenitore card -->
        <ul class="help_section_card_container">
          <!-- Singola card -->
          <li
            v-for="(card, i) in listHelpCard"
            :key="i"
            class="help_section_card"
            @mouseover="onOverChangeIndex(i)"
          >
            <div class="card_image">
              <img
                :src="
                  require('@/assets/home-business-service-slide-' +
                    card.imagePath +
                    '-480x298.jpg')
                "
                alt="avatar image"
              />
            </div>
            <div class="card_text">
              <h4 class="m_bottom">{{ card.title }}</h4>
              <p class="m_bottom">{{ card.text }}</p>
            </div>
            <div class="card_link">
              <a href="#">Discover Now →</a>
            </div>
          </li>
        </ul>
        <!-- Indicatori (puntini) -->
        <div class="dot_container">
          <i
            v-for="i in 3"
            :key="'dot_' + i"
            class="fa fa-circle"
            :class="currentHelpIndex === i ? 'active' : ''"
          ></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelpMain",
  data() {
    return {
      listHelpCard: [
        {
          imagePath: "01",
          title: "Consultative Training",
          text: "With a coach addressing multiple iusses that are off balance, affecting your buisness in various unconsidered ways.",
        },
        {
          imagePath: "02",
          title: "Real Deal Coaching",
          text: "Brings an exeptionally powerful opportunity. Being able to accept, to work with that opportunity.",
        },
        {
          imagePath: "03",
          title: "Advisor Training Program",
          text: "Getting high quality, enterpreneur midset driven online buisness coaching, is what is needed",
        },
      ],

      currentHelpIndex: 1,
    };
  },

  methods: {
    onOverChangeIndex(index) {
      this.currentHelpIndex = index + 1;
    },
  },
};
</script>

<style>
</style>