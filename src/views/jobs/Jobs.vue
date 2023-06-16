<template>
  <h1>Available Jobs</h1>
 <div v-for="job in jobs" :key="job.id">
    <h2>{{ job.title }}</h2>
 </div>
</template>

<script>
export default {
    data() {
        return {
            jobs: [
                {title: 'American king', id: '1', details: 'Loream'},
                {title: 'James Bond', id: '2', details: 'Loream'},
                {title: 'Mechanic Resurrection', id: '3', details: 'Loream'},
            ]
        }
    }
}
</script>

<style>

</style>