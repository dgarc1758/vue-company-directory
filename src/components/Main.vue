<script setup>
  import Mainsearch from './Mainsearch.vue'
  import MainCards from './MainCards.vue'
  import MainPagination from './MainPagination.vue'
  import MainPagination from './MainPagination.vue'
</script>
<template>
  <div class="wrapper">
    <Mainsearch />
    <MainCards />
    <MainPagination />
  </div>
</template>

<style scoped lang="postcss">
  @apply container mx-auto flex flex-col gap-4 py-4;
</style>
