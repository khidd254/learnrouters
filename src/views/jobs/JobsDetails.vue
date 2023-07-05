<template>
<div v-if="job">
  <h1>{{ job.title }}</h1>
  <p>the job id is {{ id }}</p>
  <p>{{ job.details }}</p>
</div>
<div v-else>
  <p>loading job details ...</p>
</div>
</template>

<script>
export default {
  props: ['id'],
  data() {
    return{
      job: null
    }
  },
  mounted() {
        fetch(' http://localhost:3000/jobs/' + this.id)
        .then(res => res.json())
        .then(data => this.job = data)
}
  // data() {
  //   return {
  //     id: this.$route.params.id
  //   }
  // }
}
</script>

<style>

</style>