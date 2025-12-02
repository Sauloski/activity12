<script setup>
const chuck = [
  {
    "value": "Chuck Norris can skydive into outer space."
  },
  {
    "value": "The chief export of Chuck Norris is pain."
  },
  {
    "value": "Chuck Norris doesn't read books. He stares them down until he gets the information he wants."
  },
  {
    "value": "Time waits for no man. Unless that man is Chuck Norris."
  },
  {
    "value": "If you spell Chuck Norris in Scrabble, you win. Forever."
  },
];
</script>

<template>
  <div class="container">
    <h1>Chuck Norris Jokes</h1>
    <ul>
      <li v-for="(joke, index) in chuck" :key="index">
        {{ joke.value }}
      </li>
    </ul>
  </div>
</template>

<style scoped>
.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 2rem;
  font-family: sans-serif;
  background-color: #f0f0f0;
  border-radius: 8px;
}

h1 {
  text-align: center;
  color: #333;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  background-color: #fff;
  padding: 1rem;
  margin-bottom: 0.5rem;
  border-radius: 4px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
</style>
