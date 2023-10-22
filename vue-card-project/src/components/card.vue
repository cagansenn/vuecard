<script setup>
defineProps({
  cardTitle: String,
  cardText: String,
  cardLink: String,
});
</script>

<template>
  <div class="col m-3">
    <div class="card" style="width: 18rem">
      <div class="card-body">
        <h5 class="card-title">{{ cardTitle }}</h5>
        <p class="card-text">
          {{ cardText }}
        </p>
        <a :href="cardLink" class="btn btn-primary">Go To The Link</a>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
