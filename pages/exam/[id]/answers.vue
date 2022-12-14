<template>
  <div class="relative min-w-72 m-8 mr-4 rounded-md bg-white shadow-md overflow-y-auto border">
    <div class="sticky top-0 font-semibold p-4 border-b backdrop-blur-sm bg-slate-100/30">Daftar Soal</div>
    <div class="p-4 grid grid-cols-8 gap-1">
      <NuxtLink :to="`/exam/1/question/${i}`" v-for="i in [...Array(100).keys()]" class="bg-slate-100 text-center rounded-md text-slate-600 text-sm p-1 hover:shadow hover:scale-105 transition-all duration-200 ease-in-out">{{ i+1 }}</NuxtLink>
    </div>
  </div>
  <div class="flex-1 w-full m-8 ml-4 border rounded-md bg-white shadow-md overflow-auto">
    <div class="p-4 border-b bg-[url('~/assets/images/blue-abstract.svg')] text-white font-semibold sticky top-0 bg-cover">Pertanyaan</div>
    <div class="mt-8 flex gap-4 items-start">
      <div class="bg-amber-400 text-2xl font-semibold text-white px-4 py-2 rounded-r-md">1</div>
      <div class="px-4 space-y-4">
        <div>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium aliquid assumenda aut deleniti et iusto laudantium nostrum officia qui suscipit.</div>
        <div class="space-y-4 w-2/3">
          <div v-for="i in [1, 3, 4, 4]" class="bg-slate-100 p-4 rounded-md cursor-pointer hover:shadow-md transition-all duration-300 ease-in-out">Pilihan {{ i }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  definePageMeta({
    layout: "exam"
  })
</script>

<style scoped>

</style>