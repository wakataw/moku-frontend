<template>
  <article class="max-w-screen-xl mx-auto grid px-4 xl:px-0 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 my-4 gap-4">
    <div v-if="pending" v-for="i in [1, 1, 1, 1]" class="w-full rounded-lg bg-slate-100 h-64 animate-pulse p-4 flex flex-col justify-between">
      <div class="bg-slate-300 h-6 w-full rounded-full"></div>
      <div class="bg-slate-300 h-4 w-4/5 rounded-full"></div>
      <div class="bg-slate-300 h-4 w-2/3 rounded-full"></div>
      <div class="bg-slate-300 h-4 w-2/3 rounded-full"></div>
      <div class="bg-slate-300 h-4 w-2/3 rounded-full"></div>
      <div class="bg-slate-300 h-6 w-full rounded-md"></div>
    </div>
    <CourseCard
        v-else
        :id="p.id"
        :short-description="p.shortDescription"
        :title="p.title"
        :duration="p.duration"
        :total-packages="p.totalExams"
        :start-date="p.startDate"
        v-for="p in packages"
    ></CourseCard>
  </article>
</template>

<script setup>
  const { pending, data: packages } = await useFetch("https://4a45-2001-448a-2082-35c7-b8d6-3767-67c3-7100.ap.ngrok.io/packages/", {lazy: true})
</script>

<style scoped>

</style>