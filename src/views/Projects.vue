<template>
  <div class="project">
    <projectCards />
  </div>
</template>

<script>
// @ is an alias to /src
import projectCards from "@/components/projectCards.vue";

export default {
  name: "Projects",
  components: {
    projectCards,
  },
};
</script>
<style scoped>
</style>