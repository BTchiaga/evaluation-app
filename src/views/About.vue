<template>
  <div class="about">
    <h1>This page collects some information about you</h1>
    <h3>D'ont worry every thing is anonymous</h3>
    <about-you />
    <div class="d-flex justify-center my-6">
      <v-btn elevation="2" outlined @click="gotoDemo">Go</v-btn>
    </div>
  </div>
</template>
<script>
import AboutYou from "../components/AboutYou.vue";

export default {
  name: "about",
  components: { AboutYou },

  data() {
    return {};
  },
  methods: {
    gotoDemo() {
      this.$router.push("demo");
    },
  },
};
</script>
