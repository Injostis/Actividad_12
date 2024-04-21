<template>
  <div class="container">
    <div class="row">
      <chuck-card
        v-for="(fact, index) in chuck"
        :key="index"
        :icon-url="fact.icon_url"
        :value="fact.value"
      />
    </div>
  </div>
</template>

<script>
import ChuckCard from "./components/ChuckCard.vue";

export default {
  components: {
    ChuckCard,
  },
  data() {
    return {
      chuck: [
        {
          icon_url:
            "https://hips.hearstapps.com/hmg-prod/images/gettyimages-150327735-copy.jpg",
          value: "Chuck Norris can skydive into outer space.",
        },
        {
          icon_url:
            "https://hips.hearstapps.com/hmg-prod/images/gettyimages-150327735-copy.jpg",
          value: "The chief export of Chuck Norris is pain.",
        },
        {
          icon_url:
            "https://hips.hearstapps.com/hmg-prod/images/gettyimages-150327735-copy.jpg",
          value:
            "Chuck Norris doesn't read books. He stares them down until he gets the information he wants.",
        },
        {
          icon_url:
            "https://hips.hearstapps.com/hmg-prod/images/gettyimages-150327735-copy.jpg",
          value: "Time waits for no man. Unless that man is Chuck Norris.",
        },
        {
          icon_url:
            "https://hips.hearstapps.com/hmg-prod/images/gettyimages-150327735-copy.jpg",
          value: "If you spell Chuck Norris in Scrabble, you win. Forever.",
        },
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
