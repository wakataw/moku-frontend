<template>
  <div class="text-slate-900 group rounded-md border overflow-hidden hover:shadow-lg transition-all duration-300 ease-in-out">
    <div class="space-y-4 p-4">
      <div>
        <h3 class="font-semibold">Uji Kompetensi Kenaikan Jenjang</h3>
      </div>
      <div class="text-slate-600 text-sm space-y-2">
        <div class="flex text-xs items-center gap-1 text-slate-500">
          <ClockIcon class="h-5 w-5"></ClockIcon>
          <span>60 menit</span>
          <span>&middot;</span>
          <DocumentIcon class="h-5 w-5"></DocumentIcon>
          <span>100 soal</span>
        </div>
      </div>
    </div>
    <div class="p-4 pt-0 items-center text-slate-600 flex justify-between">
      <NuxtLink :to="`/exam/${randomId}/`" class="bg-blue-50 text-blue-700 rounded-md p-2 flex space-x-2 items-center w-full justify-center hover:shadow transition-all duration-200 ease-in-out">
        <span>Buka</span>
        <ArrowRightOnRectangleIcon class="h-5 w-5"></ArrowRightOnRectangleIcon>
      </NuxtLink>
    </div>
  </div>
</template>

<script>
import { ClockIcon, ClipboardIcon, ArrowRightOnRectangleIcon, DocumentIcon } from '@heroicons/vue/24/outline'
import { ClipboardDocumentCheckIcon } from "@heroicons/vue/24/solid";

export default {
  name: "ModulVCard",
  props: ["randomId"],
  components: {
    ClockIcon,
    ClipboardIcon,
    ArrowRightOnRectangleIcon,
    ClipboardDocumentCheckIcon,
    DocumentIcon
  }
}
</script>

<style scoped>

</style>