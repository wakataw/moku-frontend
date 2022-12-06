<template>
  <div class="bg-[url('~/assets/images/blue-abstract.svg')] bg-cover px-4 py-8">
    <div class="max-w-screen-xl mx-auto w-full h-full py-4 flex space-x-24">
      <div class="w-1/2 space-y-4">
        <h1 class="text-2xl font-semibold text-white">Uji Kompetensi Kenaikan Jenjang Fungsional Pemeriksa Pajak</h1>
        <div class="text-slate-400 text-sm">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Enim minima molestiae omnis praesentium quae quisquam. Adipisci architecto asperiores aspernatur assumenda esse expedita fugit in modi, nemo obcaecati officiis perferendis perspiciatis quae quaerat, quo quod repellendus repudiandae sint ut vitae! At consequuntur cumque deleniti dignissimos doloremque dolores eveniet laborum sint velit?</div>
      </div>
      <div class="flex flex-col justify-between w-1/2">
        <DescriptionItem title="Waktu" subtitle="90 Menit">
          <ClockIcon class="w-8 h-8"></ClockIcon>
        </DescriptionItem>
        <DescriptionItem title="Paket" subtitle="1 tes">
          <ClipboardDocumentCheckIcon class="w-8 h-8"></ClipboardDocumentCheckIcon>
        </DescriptionItem>
        <DescriptionItem title="Jadwal" subtitle="6 Desember 2022">
          <CalendarDaysIcon class="w-8 h-8"></CalendarDaysIcon>
        </DescriptionItem>
      </div>
    </div>
  </div>
</template>

<script>
import { CalendarDaysIcon, ClockIcon, ClipboardDocumentCheckIcon } from '@heroicons/vue/24/outline'
import DescriptionItem from "./course/DescriptionItem";

export default {
  name: "CourseHeader",
  components: {
    DescriptionItem,
    ClockIcon,
    CalendarDaysIcon,
    ClipboardDocumentCheckIcon
  }
}
</script>

<style scoped>

</style>