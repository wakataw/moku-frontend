<template>
  <div class="text-slate-900 group rounded-md border overflow-hidden hover:shadow-lg transition-all duration-300 ease-in-out flex flex-col">
    <div class="flex-1 space-y-4 p-4 border-b flex flex-col">
      <div>
        <h3 class="font-semibold">{{ title }}</h3>
        <span class="text-xs bg-amber-300 text-amber-900 px-2 py-1 rounded-md">ukom</span>
      </div>
      <div class="flex-1 text-slate-600 text-sm space-y-2 flex flex-col">
        <div class="flex-1">{{ shortDescription }}</div>
        <div class="flex text-xs items-center gap-1 text-slate-500 flex-none">
          <ClockIcon class="h-5 w-5"></ClockIcon>
          <span>{{ duration }}</span>
          <span>&middot;</span>
          <ClipboardIcon class="h-5 w-5"></ClipboardIcon>
          <span>{{ totalPackages }} paket</span>
        </div>
      </div>
    </div>
    <div class="text-xs p-4 items-center text-slate-600 flex justify-between">
      <span>{{ startDate }}</span>
      <NuxtLink :to="`/ujian/${id}/`" class="bg-blue-50 text-blue-700 rounded-md p-2">
        <ArrowRightIcon class="h-5 w-5"></ArrowRightIcon>
      </NuxtLink>
    </div>
  </div>
</template>

<script setup>
import { ClockIcon, ClipboardIcon, ArrowRightIcon } from '@heroicons/vue/24/outline'

defineProps({
  id: Number,
  title: String,
  shortDescription: String,
  duration: Number,
  totalPackages: Number,
  startDate: String,
})


</script>

<style scoped>

</style>