<!-- @format -->

<template>
  <div class="md:hidden">
    <Sheet>
      <SheetTrigger>
        <div class="ml-4"><AlignJustify /></div>
      </SheetTrigger>
      <SheetTitle>
        <SheetDescription>
          <SheetContent side="left" class="bg-slate-700 text-green-200 mt-14">
            <NuxtLink to="/">
              <Icon name="ic:sharp-apple" color="green" size="46" />
            </NuxtLink>
            <nav class="flex flex-col gap-3 lg:gap-4 mt-6">
              <NuxtLink class="my-link" to="/"> Home </NuxtLink>
              <NuxtLink class="my-link" to="/about"> About </NuxtLink>
              <NuxtLink class="my-link" to="/contact"> Contact </NuxtLink>
              <NuxtLink class="my-link" to="/admin"> Dashboard </NuxtLink>
            </nav>
          </SheetContent>
        </SheetDescription>
      </SheetTitle>
    </Sheet>
  </div>
</template>

<script setup lang="ts">
import {
  Sheet,
  SheetContent,
  SheetDescription,
  // SheetHeader,
  SheetTitle,
  SheetTrigger,
} from "@/components/ui/sheet";
import { AlignJustify } from "lucide-vue-next";

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
