<template>
  <h1>Jobs details page</h1>
  <p>the job id is {{ $route.params.id }}</p>
</template>

<script>
export default {
  props: ['id'],
  // data() {
  //   return {
  //     id: this.$route.params.id
  //   }
  // }
}
</script>

<style>

</style>