<template>
  <div class="bg-[url('~/assets/images/blue-abstract.svg')] bg-cover px-4 py-8">
    <div class="max-w-screen-xl mx-auto w-full h-full py-4 flex space-x-24">
      <div class="w-1/2 space-y-4">
        <h1 class="text-2xl font-semibold text-white">{{title}}</h1>
        <div class="text-slate-400 text-sm">{{longDescription}}</div>
      </div>
      <div class="flex flex-col w-1/2 space-y-4">
        <DescriptionItem title="Waktu" :subtitle="`${duration/60} menit`">
          <ClockIcon class="w-8 h-8"></ClockIcon>
        </DescriptionItem>
        <DescriptionItem title="Paket" :subtitle="`${totalExams} paket`">
          <ClipboardDocumentCheckIcon class="w-8 h-8"></ClipboardDocumentCheckIcon>
        </DescriptionItem>
        <DescriptionItem title="Jadwal" :subtitle="startDate">
          <CalendarDaysIcon class="w-8 h-8"></CalendarDaysIcon>
        </DescriptionItem>
      </div>
    </div>
  </div>
</template>

<script setup>
import { CalendarDaysIcon, ClockIcon, ClipboardDocumentCheckIcon } from '@heroicons/vue/24/outline'
import DescriptionItem from "./course/DescriptionItem";

defineProps({
  title: String,
  longDescription: String,
  duration: Number,
  totalExams: Number,
  startDate: String,
})

</script>

<style scoped>

</style>