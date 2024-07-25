<script lang="ts" setup>
import {
  Tooltip,
  TooltipContent,
  TooltipProvider,
  TooltipTrigger,
} from "@/components/ui/tooltip";

const items = ref([
  {
    title: "Javascript",
    description: "Javascript",
    icon: " akar-icons:javascript-fill",
  },
  {
    title: "Vue Js",
    description: "Vue Js",
    icon: "nonicons:vue-16",
  },
  {
    title: "Nuxt Js",
    description: "Nuxt Js",
    icon: "tabler:brand-nuxt",
  },
  {
    title: "PHP",
    description: "PHP",
    icon: "material-symbols:php-sharp",
  },
  {
    title: "Laravel",
    description: "Laravel",
    icon: "simple-icons:laravel",
  },
  {
    title: "Tailwind CSS",
    description: "Tailwind CSS",
    icon: "ri:tailwind-css-fill",
  },
]);
</script>

<template>
  <div class="mb-10 flex pt-10">
    <div class="mx-auto">
      <h1 class="text-6xl font-bold text-white">Skills</h1>
      <iconify-icon icon="ri:tailwind-css-fill"></iconify-icon>
    </div>
  </div>
  <div class="grid grid-cols-3 gap-[30px] text-white">
    <TooltipProvider>
      <Tooltip>
        <TooltipTrigger v-for="item in items">{{ item.icon }}</TooltipTrigger>
        <TooltipContent v-for="item in items" class="bg-[#232329]">
          <p>{{ item.description }}</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
  </div>
</template>
