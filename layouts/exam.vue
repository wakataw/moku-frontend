<template>
  <div class="relative flex flex-col bg-[url('~/assets/images/bg.svg')] bg-repeat bg-slate-100/50">
    <nav class="h-16 flex items-center p-4 shadow-md justify-between sticky top-0 right-0 left-0 bg-white">
      <div class="flex items-center gap-4">
        <NuxtLink to="/ujian/1" class="bg-slate-200 p-2 rounded-md">
          <ChevronLeftIcon class="h-6 w-6"></ChevronLeftIcon>
        </NuxtLink>
        <NavLogo></NavLogo>
      </div>
      <h1 class="font-semibold text-slate-900 text-lg">Uji Kompetensi Kenaikan Peringkat Jabatan</h1>
      <div>
        <div class="bg-rose-500 text-white px-4 py-2 rounded-md font-semibold text-2xl">
          01:30:01
        </div>
      </div>
    </nav>
    <div class="flex h-screen -mt-16 pt-16">
      <slot></slot>
    </div>
  </div>
</template>

<script>
import NavLogo from "../components/NavLogo";
import { ChevronLeftIcon } from '@heroicons/vue/24/outline'
export default {
  name: "exam",
  components: {NavLogo, ChevronLeftIcon}
}
</script>

<style scoped>

</style>