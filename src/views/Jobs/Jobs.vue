<template>
  <h1>Jobs</h1>
  <div v-for="(job, index) in jobs" :key="index">
    <router-link :to="{}">
      {{ job.title }}
    </router-link>
  </div>
</template>

<script>
export default {
  name: "Jobs",
  data() {
    return {
      jobs: [
        { title: "UX Designer", id: 1, deatils: "lorem" },
        { title: "Web Developer", id: 2, deatils: "lorem" },
        { title: "Vue Developer", id: 3, deatils: "lorem" },
      ],
    };
  },
};
</script>

<style></style>
