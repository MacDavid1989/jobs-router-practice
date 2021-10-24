<template>
  <h1>Jobs</h1>
  <div v-for="(job, index) in jobs" :key="index" class="job">
    <router-link :to="{ name: 'JobDetails', params: { id: job.id } }">
      <h2>
        {{ job.title }}
      </h2>
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

<style scoped>
.job h2 {
  background: #f4f4f4;
  padding: 20px;
  border-radius: 10px;
  margin: 10px auto;
  max-width: 600px;
  cursor: pointer;
  color: #444;
}
.job h2:hover {
  background: #ddd;
}
.job a {
  text-decoration: none;
}
</style>
