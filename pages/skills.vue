<script lang="ts" setup>
import {
  Tooltip,
  TooltipContent,
  TooltipProvider,
  TooltipTrigger,
} from "@/components/ui/tooltip";
import { Icon } from "@iconify/vue";

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
        <TooltipTrigger><Icon icon="akar-icons:javascript-fill" /></TooltipTrigger>
        <TooltipContent>
          <p>Javascript</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider>
      <Tooltip>
        <TooltipTrigger><Icon icon="fa6-brands:vuejs" /></TooltipTrigger>
        <TooltipContent>
          <p>Vue Js</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider>
      <Tooltip>
        <TooltipTrigger><Icon icon="tabler:brand-nuxt" /></TooltipTrigger>
        <TooltipContent>
          <p>Nuxt Js</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
  </div>
  <div class="grid grid-cols-3 gap-[30px] text-white">
    <TooltipProvider>
      <Tooltip>
        <TooltipTrigger><Icon icon="ri:tailwind-css-fill" /></TooltipTrigger>
        <TooltipContent>
          <p>Tailwind CSS</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider>
      <Tooltip>
        <TooltipTrigger><Icon icon="material-symbols:php-sharp" /></TooltipTrigger>
        <TooltipContent>
          <p>PHP</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider>
      <Tooltip>
        <TooltipTrigger><Icon icon="simple-icons:laravel" /></TooltipTrigger>
        <TooltipContent>
          <p>Laravel</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
  </div>
</template>
