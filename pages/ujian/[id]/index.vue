<template>
  <CourseHeader
      :title="examPackages.title"
      :long-description="examPackages.longDescription"
      :duration="examPackages.duration"
      :total-exams="examPackages.totalExams"
      :start-date="examPackages.startDate"
  >
  </CourseHeader>
  <div class="max-w-screen-xl mx-auto py-4 space-y-4">
    <h2 class="text-2xl font-semibold underline decoration-yellow-400 decoration-4">Daftar Ujian</h2>
    <article class="max-w-screen-xl mx-auto grid px-4 xl:px-0 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 my-4 gap-4">
      <modul-v-card :id="i.id"
                    :title="i.title"
                    :duration="i.duration"
                    :questions="i.totalQuestions"
                    v-for="i in examPackages.exams"
      ></modul-v-card>
    </article>
  </div>
</template>

<script setup>
  import ModulVCard from "../../../components/ModulVCard";

  definePageMeta({
    layout: "course",
  })

  const id = useRoute().params.id;
  const { data: examPackages } = await useFetch(`https://4a45-2001-448a-2082-35c7-b8d6-3767-67c3-7100.ap.ngrok.io/packages/${id}?_embed=exams`)

</script>

<style scoped>

</style>