<script lang="ts" setup>
import {
  Tooltip,
  TooltipContent,
  TooltipProvider,
  TooltipTrigger,
} from "@/components/ui/tooltip";
import { Icon } from "@iconify/vue";
</script>

<template>
  <div class="mb-10 flex pt-10">
    <div class="mx-auto">
      <h1 class="text-6xl font-bold text-white">Skills</h1>
    </div>
  </div>

  <div class="grid grid-cols-3 gap-[30px] text-white basis-1/2">
    <TooltipProvider class="flex items-center justify-center bg-slate-400">
      <Tooltip>
        <TooltipTrigger
          ><Icon icon="akar-icons:javascript-fill" class="h-24 w-16 mx-auto"
        />Javascript</TooltipTrigger>
        <TooltipContent>
          <p>Javascript</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          ><Icon icon="fa6-brands:vuejs" class="h-24 w-16 mx-auto"
        />Vue Js</TooltipTrigger>
        <TooltipContent>
          <p>Vue Js</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          ><Icon icon="tabler:brand-nuxt" class="h-24 w-16 mx-auto"
        />Nuxt Js</TooltipTrigger>
        <TooltipContent>
          <p>Nuxt Js</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
  </div>

  <div class="my-10 grid grid-cols-3 gap-[30px] text-white">
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          ><Icon icon="ri:tailwind-css-fill" class="h-24 w-16 mx-auto"
        />Tailwind CSS</TooltipTrigger>
        <TooltipContent>
          <p>Tailwind CSS</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          ><Icon icon="material-symbols:php-sharp" class="h-24 w-16 mx-auto"
        />PHP</TooltipTrigger>
        <TooltipContent>
          <p>PHP</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          ><Icon icon="simple-icons:laravel" class="h-24 w-16 mx-auto"
        />Laravel</TooltipTrigger>
        <TooltipContent>
          <p>Laravel</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
  </div>
  
  <div class="my-10 grid grid-cols-3 gap-[30px] text-white">
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          ><Icon icon="file-icons:sqlite" class="h-24 w-16 mx-auto"
        />SQLite</TooltipTrigger>
        <TooltipContent>
          <p>SQLite</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          ><Icon icon="gg:figma" class="h-24 w-16 mx-auto"
        />Figma</TooltipTrigger>
        <TooltipContent>
          <p>Figma</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          ><Icon icon="bi:git" class="h-24 w-16 mx-auto"
        />Git</TooltipTrigger>
        <TooltipContent>
          <p>Git</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
  </div>
</template>
