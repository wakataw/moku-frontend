<template>
  <div class="max-w-screen-xl mx-auto py-4 space-y-4">
    <h2 class="text-2xl font-semibold underline decoration-yellow-400 decoration-4">Daftar Ujian</h2>
    <article class="max-w-screen-xl mx-auto grid px-4 xl:px-0 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 my-4 gap-4">
      <modul-v-card :random-id="i" v-for="i in [1, 2]" ></modul-v-card>
    </article>
  </div>
</template>

<script setup>
  import ModulVCard from "../../../components/ModulVCard";

  definePageMeta({
    layout: "course",
  })

</script>

<style scoped>

</style>