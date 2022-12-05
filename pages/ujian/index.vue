<template>
  <article class="max-w-screen-xl mx-auto grid px-4 xl:px-0 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 my-4 gap-4">
    <CourseCard :random-id="i" v-for="i in [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]"></CourseCard>
  </article>
</template>

<script>

export default {
  name: "index",
  components: {}

}
</script>

<style scoped>

</style>