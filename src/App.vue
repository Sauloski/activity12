<script setup>
import ChuckCard from './components/ChuckCard.vue'

const chuck = [
  {
    "icon_url": "https://pngimg.com/uploads/chuck_norris/chuck_norris_PNG30.png",
    "value": "Chuck Norris can skydive into outer space."
  },
  {
    "icon_url": "https://pngimg.com/uploads/chuck_norris/chuck_norris_PNG19.png",
    "value": "The chief export of Chuck Norris is pain."
  },
  {
    "icon_url": "https://pngimg.com/uploads/chuck_norris/chuck_norris_PNG23.png",
    "value": "Chuck Norris doesn't read books. He stares them down until he gets the information he wants."
  },
  {
    "icon_url": "https://pngimg.com/uploads/chuck_norris/chuck_norris_PNG28.png",
    "value": "Time waits for no man. Unless that man is Chuck Norris."
  },
  {
    "icon_url": "https://pngimg.com/uploads/chuck_norris/chuck_norris_PNG10.png",
    "value": "If you spell Chuck Norris in Scrabble, you win. Forever."
  },
];
</script>

<template>
  <div class="container my-5">
    <h1 class="text-center mb-4">Chuck Norris Jokes</h1>
    <div class="row">
      <div v-for="(joke, index) in chuck" :key="index" class="col-12 col-md-4 mb-4">
        <ChuckCard :icon_url="joke.icon_url" :value="joke.value" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  max-width: 960px;
}

h1 {
  font-family: 'Anton', sans-serif;
  color: #2c3e50;
}
</style>
