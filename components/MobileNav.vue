<script lang="ts" setup>
import {
  Sheet,
  SheetClose,
  SheetContent,
  SheetDescription,
  SheetFooter,
  SheetHeader,
  SheetTitle,
  SheetTrigger,
} from "@/components/ui/sheet";

import { Icon } from "@iconify/vue";
</script>

<template>
  <Sheet>
    <SheetTrigger class="flex items-center justify-center">
      <Icon icon="mingcute:menu-fill" class="text-[32px]"/>
    </SheetTrigger>
    <SheetContent class="flex flex-col bg-primary">
      <!-- Logo -->
      <div class="mb-40 mt-32 text-center">
        <NuxtLink to="/" class="text-4xl font-extrabold text-white"
          >Ye Hong<span class="text-blue-500">.</span>
        </NuxtLink>
      </div>

      <!-- Nav -->
      <nav class="flex flex-col items-center justify-center gap-8 text-white text-2xl">
        <NuxtLink
          to="/experience"
          class="border-blue-500 hover:border-b-2 hover:text-blue-500"
          >Experiences</NuxtLink
        >
        <NuxtLink
          to="/education"
          class="border-blue-500 hover:border-b-2 hover:text-blue-500"
          >Education</NuxtLink
        >
        <NuxtLink
          to="/skills"
          class="border-blue-500 hover:border-b-2 hover:text-blue-500"
          >Skills</NuxtLink
        >
        <NuxtLink
          to="/projects"
          class="border-blue-500 hover:border-b-2 hover:text-blue-500"
          >Projects</NuxtLink
        >
      </nav>
    </SheetContent>
  </Sheet>
</template>
