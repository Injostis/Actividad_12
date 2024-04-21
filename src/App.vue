<script setup>
import HelloWorld from "./components/HelloWorld.vue";
import TheWelcome from "./components/TheWelcome.vue";
</script>

<template>
  <div id="app">
    <h1>Chuck Norris Facts</h1>
    <ul>
      <li v-for="(fact, index) in chuck" :key="index">
        {{ fact.value }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      chuck: [
        { value: "Chuck Norris can skydive into outer space." },
        { value: "The chief export of Chuck Norris is pain." },
        {
          value:
            "Chuck Norris doesn't read books. He stares them down until he gets the information he wants.",
        },
        { value: "Time waits for no man. Unless that man is Chuck Norris." },
        { value: "If you spell Chuck Norris in Scrabble, you win. Forever." },
      ],
    };
  },
};
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1 {
  font-size: 2em;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  margin: 10px 0;
  font-size: 1.2em;
}
</style>
