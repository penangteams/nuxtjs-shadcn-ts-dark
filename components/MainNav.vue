<!-- @format -->

<template>
  <div class="hidden md:flex">
    <NuxtLink to="/">
      <Icon name="ic:sharp-apple" color="green" size="46" />
    </NuxtLink>
    <nav class="flex items-center gap-3 lg:gap-4 ml-4">
      <NuxtLink class="my-link" to="/"> Home </NuxtLink>
      <NuxtLink class="my-link" to="/about"> About </NuxtLink>
      <NuxtLink class="my-link" to="/contact"> Contact </NuxtLink>
      <NuxtLink class="my-link" to="/admin"> Dashboard </NuxtLink>
    </nav>
  </div>
</template>

<script setup lang="ts">
defineProps({
  to: {
    type: String,
  },
});
</script>
<style scoped>
.my-link.router-link-active {
  @apply bg-orange-100 text-orange-600 rounded px-2 py-2;
}
.my-link.router-link-active:hover {
  @apply px-2 py-2;
}
</style>
