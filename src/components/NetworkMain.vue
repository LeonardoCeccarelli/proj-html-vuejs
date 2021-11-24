<template>
  <div>
    <div class="network_container">
      <!-- Immagini position absolute -->
      <img
        class="background_globe"
        src="@/assets/background-map-dots-top-right-transparent.png"
        alt="globe image"
      />
      <img
        class="background_cube"
        src="@/assets/maxcoach-shape-07.png"
        alt="cube_image"
      />
      <div class="network_content">
        <div class="network_image_container">
          <!-- Sezione immagine con logo youtube al centro -->
          <div class="network_image">
            <img
              src="@/assets/home-business-video-poster-670x450.jpg"
              alt="youtube video"
            />

            <img
              src="@/assets/icon-youtube-play.png"
              alt="logo youtube"
              class="logo_play"
            />
          </div>
        </div>
        <div class="network_text_container">
          <!-- Sezione testo -->
          <div class="network_text_content">
            <h2>To Trive In Buisness Today, You'll Need a Good Plan</h2>
            <!-- Singolo dropdown menu -->
            <div
              v-for="(question, i) in listQuestion"
              :key="i"
              class="question_container"
              :class="i === currentQuestionActive ? 'active' : ''"
              @click="onClickChangeQuestion(i)"
            >
              <h4 class="question_title m_bottom">
                <i class="fa fa-chevron-circle-down"></i>{{ question.title }}
              </h4>
              <div class="question_text">
                <p class="m_bottom">{{ question.textTop }}</p>
                <p class="m_bottom">{{ question.textBottom }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NetworkMain",
  data() {
    return {
      listQuestion: [
        {
          title: "How can we help?",
          textTop:
            "How many courses you've been on, using however many techniques and methods. Unless you've come to rendize the value of mindset, then you've get to understand how succes comes.",
          textBottom:
            "With everyone else's mindset involving impacted too. Hence why buisness coaching is so crucial for succes.",
        },
        {
          title: "Why would i need a buisness COACH?",
          textTop:
            "How many courses you've been on, using however many techniques and methods. Unless you've come to rendize the value of mindset, then you've get to understand how succes comes.",
          textBottom:
            "With everyone else's mindset involving impacted too. Hence why buisness coaching is so crucial for succes.",
        },
        {
          title: "What is one-to-one coaching?",
          textTop:
            "How many courses you've been on, using however many techniques and methods. Unless you've come to rendize the value of mindset, then you've get to understand how succes comes.",
          textBottom:
            "With everyone else's mindset involving impacted too. Hence why buisness coaching is so crucial for succes.",
        },
      ],

      currentQuestionActive: 0,
    };
  },
  methods: {
    onClickChangeQuestion(index) {
      this.currentQuestionActive = index;
    },
  },
};
</script>

<style>
</style>