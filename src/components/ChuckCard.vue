<script setup>
defineProps({
  icon_url: {
    type: String,
    required: true
  },
  value: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="card h-100">
    <img :src="icon_url" class="card-img-top w-50 mx-auto mt-3" alt="Chuck Norris">
    <div class="card-body d-flex flex-column">
      <p class="card-text">{{ value }}</p>
    </div>
  </div>
</template>

<style scoped>
.card-text {
  font-size: 1.1rem;
  text-align: center;
  margin-top: auto;
}
</style>
