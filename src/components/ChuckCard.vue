<template>
  <div>
    <img
      :src="iconUrl"
      alt="Chuck Norris Fact"
      style="width: 50px; height: 50px"
    />
    <p>{{ value }}</p>
  </div>
</template>

<script>
export default {
  props: {
    iconUrl: String,
    value: String,
  },
};
</script>
