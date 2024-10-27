<!-- @format -->

<template>
  <header class="sticks top-0 w-full bg-[#007984] text-[#18D788]">
    <div class="h-14 flex items-center">
      <!-- Desktop  -->
      <MainNav />

      <!-- Mobile  -->
      <MobileNav />

      <!-- Desktop & mobile  -->
      <div class="flex justify-start flex-1 ml-3">
        <!-- <Searchbox /> -->
      </div>
      <h1 class="flex items-center justify-end flex-1">
        <ModeToggle />
      </h1>
    </div>
  </header>
</template>
