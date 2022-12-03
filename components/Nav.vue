<template>
  <nav class="shadow-md">
    <div class="max-w-screen-xl mx-auto p-2 xl:px-0 flex justify-between items-center gap-4 h-16">
      <a href="" class="h-10 flex gap-1 items-center text-slate-600 text-2xl">
        <img src="~/assets/images/logo.png" alt="" class="h-full">
        <span>studia</span>
      </a>
      <div class="relative flex-1 w-full">
        <label for="">
          <MagnifyingGlassIcon class="h-6 w-6 absolute text-slate-400 right-2 top-2"></MagnifyingGlassIcon>
        </label>
        <input type="text" class="bg-slate-200 px-4 py-2 rounded-md outline-none placeholder:text-slate-400 w-full" placeholder="Cari ...">
      </div>
      <div class="flex gap-4 items-center">
        <div class="flex gap-2">
          <button class="text-sm items-center h-10 flex gap-1 text-slate-600 hover:bg-blue-50 hover:text-blue-500 px-2 py-2 rounded-md">
            <BookOpenIcon class="mx-auto h-6 w-6"></BookOpenIcon>
            <span>Kursus</span>
          </button>
          <button class="text-sm items-center h-10 flex gap-1 text-slate-600 hover:bg-blue-50 hover:text-blue-500 px-2 py-2 rounded-md">
            <ClipboardDocumentCheckIcon class="mx-auto h-6 w-6"></ClipboardDocumentCheckIcon>
            <span>Ujian</span>
          </button>
        </div>
        <button class="bg-blue-50 text-blue-700 rounded-md px-3 py-2 flex items-center text-sm gap-2 h-10">
          <span>Agung Pratama</span>
          <ChevronDownIcon class="h-4 w-4"></ChevronDownIcon>
        </button>
      </div>
    </div>
  </nav>
</template>

<script>
import { MagnifyingGlassIcon, ChevronDownIcon, ClipboardDocumentCheckIcon, BookOpenIcon } from '@heroicons/vue/24/outline'

export default {
  name: "Nav",
  components : {
    MagnifyingGlassIcon,
    ClipboardDocumentCheckIcon,
    ChevronDownIcon,
    BookOpenIcon
  }
}
</script>
