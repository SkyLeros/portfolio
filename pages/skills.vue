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
  <div
    class="grid grid-cols-1 gap-4 p-4 mx-4 text-white sm:grid-cols-2 sm:mx-6 md:grid-cols-3 md:mx-10 lg:mx-20 lg:gap-6 "
  >
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          class="rounded-md border-2 border-gray-500 p-4 hover:bg-slate-600"
        >
          <Icon
            icon="akar-icons:javascript-fill"
            class="mx-auto h-16 w-16 md:h-24 md:w-24"
          />
          <span class="mt-2 block text-center">Javascript</span>
        </TooltipTrigger>
        <TooltipContent>
          <p class="text-center">Javascript</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          class="rounded-md border-2 border-gray-500 p-4 hover:bg-slate-600"
        >
          <Icon
            icon="fa6-brands:vuejs"
            class="mx-auto h-16 w-16 md:h-24 md:w-24"
          />
          <span class="mt-2 block text-center">Vue Js</span>
        </TooltipTrigger>
        <TooltipContent>
          <p class="text-center">Vue Js</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          class="rounded-md border-2 border-gray-500 p-4 hover:bg-slate-600"
        >
          <Icon
            icon="tabler:brand-nuxt"
            class="mx-auto h-16 w-16 md:h-24 md:w-24"
          />
          <span class="mt-2 block text-center">Nuxt Js</span>
        </TooltipTrigger>
        <TooltipContent>
          <p class="text-center">Nuxt Js</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>

    <!-- Second Row -->
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          class="rounded-md border-2 border-gray-500 p-4 hover:bg-slate-600"
        >
          <Icon
            icon="ri:tailwind-css-fill"
            class="mx-auto h-16 w-16 md:h-24 md:w-24"
          />
          <span class="mt-2 block text-center">Tailwind CSS</span>
        </TooltipTrigger>
        <TooltipContent>
          <p class="text-center">Tailwind CSS</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          class="rounded-md border-2 border-gray-500 p-4 hover:bg-slate-600"
        >
          <Icon
            icon="material-symbols:php-sharp"
            class="mx-auto h-16 w-16 md:h-24 md:w-24"
          />
          <span class="mt-2 block text-center">PHP</span>
        </TooltipTrigger>
        <TooltipContent>
          <p class="text-center">PHP</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          class="rounded-md border-2 border-gray-500 p-4 hover:bg-slate-600"
        >
          <Icon
            icon="simple-icons:laravel"
            class="mx-auto h-16 w-16 md:h-24 md:w-24"
          />
          <span class="mt-2 block text-center">Laravel</span>
        </TooltipTrigger>
        <TooltipContent>
          <p class="text-center">Laravel</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>

    <!-- Third row -->
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          class="rounded-md border-2 border-gray-500 p-4 hover:bg-slate-600"
        >
          <Icon
            icon="file-icons:sqlite"
            class="mx-auto h-16 w-16 md:h-24 md:w-24"
          />
          <span class="mt-2 block text-center">SQLite</span>
        </TooltipTrigger>
        <TooltipContent>
          <p class="text-center">SQLite</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          class="rounded-md border-2 border-gray-500 p-4 hover:bg-slate-600"
        >
          <Icon icon="gg:figma" class="mx-auto h-16 w-16 md:h-24 md:w-24" />
          <span class="mt-2 block text-center">Figma</span>
        </TooltipTrigger>
        <TooltipContent>
          <p class="text-center">Figma</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
    <TooltipProvider class="flex items-center justify-center">
      <Tooltip>
        <TooltipTrigger
          class="rounded-md border-2 border-gray-500 p-4 hover:bg-slate-600"
        >
          <Icon icon="bi:git" class="mx-auto h-16 w-16 md:h-24 md:w-24" />
          <span class="mt-2 block text-center">Git</span>
        </TooltipTrigger>
        <TooltipContent>
          <p class="text-center">Git</p>
        </TooltipContent>
      </Tooltip>
    </TooltipProvider>
  </div>
</template>
