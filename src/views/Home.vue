<template>
  <div class="project">
    <start id="start" />
    <aboutBlock id="about" />
    <projectCards id="projects" />
    <contactForm id="contact" />
  </div>
</template>

<script>
// @ is an alias to /src
import projectCards from "@/components/projectCards.vue";
import AboutBlock from "../components/aboutBlock.vue";
import contactForm from "../components/contactForm.vue";
import start from "../components/start.vue";

export default {
  name: "Home",
  components: {
    start,
    projectCards,
    AboutBlock,
    contactForm,
  },
};
</script>
<style scoped>
</style>