<template>
  <div>
    <div class="review_container">
      <div class="review_content">
        <!-- Sezione titolo -->
        <div class="review_title_container">
          <p class="head_title m_bottom">People are praising Maxcoach</p>
          <h2>What make the love us?</h2>
        </div>
        <!-- Lista commenti da utenti -->
        <ul class="review_card_container">
          <!-- Singola recensione -->
          <li
            @mouseover="onChangeActiveImage(i)"
            v-for="(user, i) in listUserReview"
            :key="i"
            class="review_single_card"
            :class="currentUserActive === i ? 'active' : ''"
          >
            <p class="title_review m_bottom">{{ user.titleReview }}</p>
            <p class="content_review">{{ user.contentReview }}</p>
            <div class="user_container">
              <!-- Immagine utente -->
              <img
                class="user_image"
                :src="
                  require('@/assets/testimonial-avata-' +
                    user.imagePath +
                    '.jpg')
                "
                alt="user image"
              />
              <div class="user_text">
                <p class="user_name">{{ user.name }}</p>
                <p class="user_type">/{{ user.type }}</p>
              </div>
            </div>
          </li>
        </ul>
        <!-- Indicatori (puntini) -->
        <div class="dot_container">
          <i
            @click="onChangeActiveImage(i)"
            v-for="(user, i) in listUserReview"
            :key="'dot n_' + i"
            class="fa fa-circle"
            :class="currentUserActive === i ? 'active' : ''"
          ></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ReviewMain",
  data() {
    return {
      listUserReview: [
        {
          name: "Florence Themence",
          type: "Multimedia Admin",
          imagePath: "03",
          titleReview: "It's a choice of quality for people with special needs",
          contentReview:
            "I'm a vrey strict person so I require everything to be organized and neat. Then I'll be able to make things right and shine. Maxcoach guys just got me.",
        },
        {
          name: "Mina Hollace",
          type: "Freelancer",
          imagePath: "02",
          titleReview:
            "High level of efficency and scientific teaching methods",
          contentReview:
            "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
        },
        {
          name: "Madley Pondor",
          type: "IT specialist",
          imagePath: "04",
          titleReview:
            "Professional team of specialist and passionate mentors of reach",
          contentReview:
            "I need to get a certification for English proficiency and Maxcoach is my best choice. Their tutors are smart and professional when dealing with students.",
        },
      ],

      currentUserActive: 1,
    };
  },
  methods: {
    onChangeActiveImage(index) {
      this.currentUserActive = index;
    },
  },
};
</script>

<style>
</style>