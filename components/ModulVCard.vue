<template>
  <div class="flex flex-col text-slate-900 group rounded-md border overflow-hidden hover:shadow-lg transition-all duration-300 ease-in-out">
    <div class="flex-1 flex flex-col space-y-4 p-4">
      <div class="flex-1">
        <h3 class="font-semibold">{{title}}</h3>
      </div>
      <div class="text-slate-600 text-sm space-y-2">
        <div class="flex text-xs items-center gap-1 text-slate-500">
          <ClockIcon class="h-5 w-5"></ClockIcon>
          <span>{{ duration }} menit</span>
          <span>&middot;</span>
          <DocumentIcon class="h-5 w-5"></DocumentIcon>
          <span>{{ questions }} soal</span>
        </div>
      </div>
    </div>
    <div class="p-4 pt-0 items-center text-slate-600 flex justify-between">
      <NuxtLink :to="`/exam/${id}/`" class="bg-blue-50 text-blue-700 rounded-md p-2 flex space-x-2 items-center w-full justify-center hover:shadow transition-all duration-200 ease-in-out">
        <span>Buka</span>
        <ArrowRightOnRectangleIcon class="h-5 w-5"></ArrowRightOnRectangleIcon>
      </NuxtLink>
    </div>
  </div>
</template>

<script setup>
import { ClockIcon, ArrowRightOnRectangleIcon, DocumentIcon } from '@heroicons/vue/24/outline'

defineProps({
  title: String,
  duration: Number,
  questions: Number,
  id: Number
})

</script>

<style scoped>

</style>