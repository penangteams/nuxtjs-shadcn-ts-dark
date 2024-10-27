<!-- @format -->

<template>
  <div class="mr-2">
    <select
      v-model="$colorMode.preference"
      class="bg-slate-600 text-white px-2 py-1"
    >
      <option value="system">System</option>
      <option value="light">Light</option>
      <option value="dark">Dark</option>
      <option value="sepia">Sepia</option>
    </select>
  </div>
</template>

<script setup lang="ts">
const colorMode = useColorMode();

console.log(colorMode.preference);
</script>

<style>
body {
  background-color: #fff;
  color: rgba(20, 3, 3, 0.8);
}
.dark-mode body {
  background-color: #091a28;
  color: #ebf4f1;
}
.sepia-mode body {
  background-color: #f1e7d0;
  color: #433422;
}
</style>
