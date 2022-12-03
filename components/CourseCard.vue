<template>
  <div class="text-slate-900 group rounded-md border overflow-hidden hover:shadow-lg transition-all duration-300 ease-in-out">
    <div class="space-y-4 p-4 border-b">
      <div>
        <h3 class="font-semibold">Uji Kompetensi Kenaikan Jenjang</h3>
        <span class="text-xs bg-amber-300 text-amber-900 px-2 py-1 rounded-md">ukom</span>
      </div>
      <div class="text-slate-600 text-sm space-y-2">
        <p>Bagi Pejabat Fungsional Pemeriksa Pajak</p>
        <div class="flex text-xs items-center gap-1 text-slate-500">
          <ClockIcon class="h-5 w-5"></ClockIcon>
          <span>60 menit</span>
          <span>&middot;</span>
          <ClipboardIcon class="h-5 w-5"></ClipboardIcon>
          <span>2 paket</span>
        </div>
      </div>
    </div>
    <div class="text-xs p-4 items-center text-slate-600 flex justify-between">
      <span>26 Oktober 2022</span>
      <button class="bg-blue-50 text-blue-700 rounded-md p-2">
        <ArrowRightIcon class="h-5 w-5"></ArrowRightIcon>
      </button>
    </div>
  </div>
</template>

<script>
import { ClockIcon, ClipboardIcon, ArrowRightIcon } from '@heroicons/vue/24/outline'
import { ClipboardDocumentCheckIcon } from "@heroicons/vue/24/solid";

export default {
  name: "CourseCard",
  props: ["randomId"],
  components: {
    ClockIcon,
    ClipboardIcon,
    ArrowRightIcon,
    ClipboardDocumentCheckIcon
  }
}
</script>

<style scoped>

</style>