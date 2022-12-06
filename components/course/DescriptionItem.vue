<template>
  <div class="flex items-center gap-4">
    <div class="bg-yellow-300 p-2 rounded-md text-yellow-900">
      <slot></slot>
    </div>
    <div>
      <div class="text-slate-400 text-sm">{{ title }}</div>
      <div class="text-white text-lg font-semibold">{{ subtitle }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "DescriptionItem",
  props: {
    title: String,
    subtitle: String,
  }
}
</script>

<style scoped>

</style>