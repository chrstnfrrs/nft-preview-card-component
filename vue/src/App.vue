<template>
  <NFTCard />
</template>

<script>
import NFTCard from "./components/NFTCard.vue";

export default {
  name: "App",
  components: {
    NFTCard,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Outfit");

html {
  font-family: Outfit, Helvetica, Arial, sans-serif;
  src: local("Outfit"), local("Outfit"),
    url(https://fonts.googleapis.com/css?family=Outfit) format("woff2");
  font-display: swap;
}

body,
p {
  margin: 0;
}
</style>
