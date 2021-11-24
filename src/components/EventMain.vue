<template>
  <div>
    <div class="event_section">
      <!-- Sezione titolo -->
      <div class="event_section_title_container">
        <p class="head_title m_bottom">Wanna transform your life?</p>
        <h2>Upcoming Events</h2>
      </div>
      <!-- Contenitore lista eventi -->
      <ul class="list_event_container">
        <!-- Singola card evento -->
        <li v-for="(event, i) in listEvent" :key="i" class="single_event">
          <!-- Linea overlay sx -->
          <div class="line_overlay"></div>
          <div class="single_event_title">
            <p class="m_bottom">
              <i class="fa fa-map-marker"></i>{{ event.place }}
            </p>
            <h3>{{ event.title }}</h3>
          </div>
          <div class="single_event_date">
            <p class="head_title day">{{ event.dateDay }}</p>
            <p class="month">{{ event.dateMonth }}</p>
            <button type="button" class="btun btun_small btun_primary">
              Get Ticket
            </button>
          </div>
        </li>
      </ul>
      <!-- Contenitore link per eventi -->
      <div class="link_bottom">
        <p>
          Exited about our event?
          <a href="#" class="link_event">View all events →</a>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "EventMain",
  data() {
    return {
      listEvent: [
        {
          title: "Storytelling Workshop",
          place: "Texas, US",
          dateDay: "22",
          dateMonth: "Nov",
        },
        {
          title: "Painting Art Contest 2020",
          place: "New York, US",
          dateDay: "10",
          dateMonth: "Oct",
        },
        {
          title: "International Art Fair 2020",
          place: "Hamburh, Germany",
          dateDay: "23",
          dateMonth: "Nov",
        },
        {
          title: "Street Performance: Call of Artist",
          place: "Illinois, US",
          dateDay: "15",
          dateMonth: "Dec",
        },
        {
          title: "Consumer Food Satefy Education Conference",
          place: "Illinoys, US",
          dateDay: "22",
          dateMonth: "Jun",
        },
        {
          title: "How meditation improve your mental healt?",
          place: "Dubai",
          dateDay: "12",
          dateMonth: "Aug",
        },
      ],
    };
  },
};
</script>

<style>
</style>