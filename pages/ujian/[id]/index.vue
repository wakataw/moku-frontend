<template>
  <h1>this is id {{ route.params.id }}</h1>
</template>

<script setup>
  import {useRoute} from "nuxt/app";

  definePageMeta({
    layout: "course",
  })

  const route = useRoute();

</script>

<style scoped>

</style>