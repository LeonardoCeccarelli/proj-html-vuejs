<template>
  <div>
    <div class="course_container">
      <div class="course_content">
        <div class="course_title">
          <p class="m_bottom head_title">Let's Dream Big Together</p>
          <h2>Explore How Can I Help You</h2>
        </div>
        <ul class="course_card_container">
          <li v-for="(card, i) in listCourseCard" :key="i" class="course_card">
            <div class="content_card">
              <img :src="require('@/assets/' + card.imagePath)" alt="" />
              <div class="content_card_text">
                <p class="price">
                  {{ card.priceInt
                  }}<small v-if="card.priceFloat">{{ card.priceFloat }}</small>
                </p>
                <p class="description m_bottom">
                  {{ card.title }}
                </p>
                <div class="on_hover_card">
                  <div class="info">
                    <span><i class="fa fa-file-text-o"></i> 20 Lessons</span>
                    <span class="last_item"
                      ><i class="fa fa-user-o"></i> 50 Students</span
                    >
                    <p class="info_description">
                      Lorem ipsum dolor, sit amet consectetur adipisicing elit.
                      Tenetur omnis itaque quasi, quam nobis beatae officiis...
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </li>
        </ul>
        <div class="course_sub_text">
          <p>
            Take the control of their life back and start doing things to make
            their dream come true. <a href="#">View all courses →</a>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CourseMain",
  data() {
    return {
      listCourseCard: [
        {
          imagePath: "course-02-443x600.jpg",
          priceInt: "$40",
          priceFloat: ".00",
          title: "Learning to Write as a Professional Author",
        },
        {
          imagePath: "stock-full-hd-03-443x600.jpg",
          priceInt: "Free",
          priceFloat: false,
          title: "Customer-Centric Info-Tech Strategies",
        },
        {
          imagePath: "stock-full-hd-04-443x600.jpg",
          priceInt: "$19",
          priceFloat: ".00",
          title: "Open Programming Courses for Everyone: Phyton",
        },
        {
          imagePath: "stock-full-hd-06-443x600.jpg",
          priceInt: "$26",
          priceFloat: ".00",
          title: "Academic LIstening and Note-taking",
        },
      ],
    };
  },
};
</script>

<style>
</style>