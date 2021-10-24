<template>
  <h1>Jobs</h1>
  <div v-for="(job, index) in jobs" :key="index">
    <h2>
      {{ job.title }}
    </h2>
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
