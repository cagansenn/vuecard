<script setup>
import { ref } from "vue";
import card from "./components/card.vue";

const cards = ref([
  {
    id: 1,
    cardTitle: "First Vue Compenent",
    cardText:
      "odio morbi quis commodo odio aenean sed adipiscing diam donec adipiscing tristique",
    cardLink: "https://google.com",
  },
  {
    id: 2,
    cardTitle: "Second Vue Compenent",
    cardText:
      "eu turpis egestas pretium aenean pharetra magna ac placerat vestibulum lectus mauris",
    cardLink: "https://youtube.com"
  },
  {
    id: 3,
    cardTitle: "Third Vue Compenent",
    cardText:
      "cras tincidunt lobortis feugiat vivamus at augue eget arcu dictum varius duis",
    cardLink: "https://vuejs.org"
  },
  {
    id: 4,
    cardTitle: "Fourth Vue Compenent",
    cardText:
      "elementum curabitur vitae nunc sed velit dignissim sodales ut eu sem integer",
    cardLink: "https://vuejs.org"
  },
]);
</script>

<template>
  <div id="card-section" class="container">
    <div class="row">
      <card
        v-for="card in cards"
        :key="card.id"
        :card-title="card.cardTitle"
        :card-text="card.cardText"
        :card-link="card.cardLink"
      ></card>
    </div>
  </div>
</template>

<style scoped></style>
