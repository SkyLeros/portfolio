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
  <div class="container mx-auto">
    <div
      class="mx-4 grid grid-cols-1 gap-6 p-4 text-white sm:mx-6 sm:grid-cols-2 md:mx-10 md:grid-cols-3 lg:mx-20 lg:gap-6"
    >
      <TooltipProvider
        class="flex items-center justify-center"
        :delayDuration="100"
      >
        <Tooltip>
          <TooltipTrigger
            class="rounded-md border-2 border-gray-500 p-4 hover:border-blue-500 hover:bg-slate-700"
          >
            <Icon
              icon="akar-icons:javascript-fill"
              class="mx-auto h-16 w-16 md:h-24 md:w-24"
            />
            <span class="mt-2 block text-center font-bold">Javascript</span>
          </TooltipTrigger>
        </Tooltip>
      </TooltipProvider>
      <TooltipProvider
        class="flex items-center justify-center"
        :delayDuration="100"
      >
        <Tooltip>
          <TooltipTrigger
            class="rounded-md border-2 border-gray-500 p-4 hover:border-blue-500 hover:bg-slate-700"
          >
            <Icon
              icon="fa6-brands:vuejs"
              class="mx-auto h-16 w-16 md:h-24 md:w-24"
            />
            <span class="mt-2 block text-center font-bold">Vue Js</span>
          </TooltipTrigger>
        </Tooltip>
      </TooltipProvider>
      <TooltipProvider
        class="flex items-center justify-center"
        :delayDuration="110"
      >
        <Tooltip>
          <TooltipTrigger
            class="rounded-md border-2 border-gray-500 p-4 hover:border-blue-500 hover:bg-slate-700"
          >
            <Icon
              icon="tabler:brand-nuxt"
              class="mx-auto h-16 w-16 md:h-24 md:w-24"
            />
            <span class="mt-2 block text-center font-bold">Nuxt Js</span>
          </TooltipTrigger>
        </Tooltip>
      </TooltipProvider>

      <!-- Second Row -->
      <TooltipProvider
        class="flex items-center justify-center"
        :delayDuration="100"
      >
        <Tooltip>
          <TooltipTrigger
            class="rounded-md border-2 border-gray-500 p-4 hover:border-blue-500 hover:bg-slate-700"
          >
            <Icon
              icon="ri:tailwind-css-fill"
              class="mx-auto h-16 w-16 md:h-24 md:w-24"
            />
            <span class="mt-2 block text-center font-bold">Tailwind CSS</span>
          </TooltipTrigger>
        </Tooltip>
      </TooltipProvider>
      <TooltipProvider
        class="flex items-center justify-center"
        :delayDuration="100"
      >
        <Tooltip>
          <TooltipTrigger
            class="rounded-md border-2 border-gray-500 p-4 hover:border-blue-500 hover:bg-slate-700"
          >
            <Icon
              icon="material-symbols:php-sharp"
              class="mx-auto h-16 w-16 md:h-24 md:w-24"
            />
            <span class="mt-2 block text-center font-bold">PHP</span>
          </TooltipTrigger>
        </Tooltip>
      </TooltipProvider>
      <TooltipProvider
        class="flex items-center justify-center"
        :delayDuration="100"
      >
        <Tooltip>
          <TooltipTrigger
            class="rounded-md border-2 border-gray-500 p-4 hover:border-blue-500 hover:bg-slate-700"
          >
            <Icon
              icon="simple-icons:laravel"
              class="mx-auto h-16 w-16 md:h-24 md:w-24"
            />
            <span class="mt-2 block text-center font-bold">Laravel</span>
          </TooltipTrigger>
        </Tooltip>
      </TooltipProvider>

      <!-- Third row -->
      <TooltipProvider
        class="flex items-center justify-center"
        :delayDuration="100"
      >
        <Tooltip>
          <TooltipTrigger
            class="rounded-md border-2 border-gray-500 p-4 hover:border-blue-500 hover:bg-slate-700"
          >
            <Icon
              icon="file-icons:sqlite"
              class="mx-auto h-16 w-16 md:h-24 md:w-24"
            />
            <span class="mt-2 block text-center font-bold">SQLite</span>
          </TooltipTrigger>
        </Tooltip>
      </TooltipProvider>
      <TooltipProvider
        class="flex items-center justify-center"
        :delayDuration="100"
      >
        <Tooltip>
          <TooltipTrigger
            class="rounded-md border-2 border-gray-500 p-4 hover:border-blue-500 hover:bg-slate-700"
          >
            <Icon icon="gg:figma" class="mx-auto h-16 w-16 md:h-24 md:w-24" />
            <span class="mt-2 block text-center font-bold">Figma</span>
          </TooltipTrigger>
        </Tooltip>
      </TooltipProvider>
      <TooltipProvider
        class="flex items-center justify-center"
        :delayDuration="100"
      >
        <Tooltip>
          <TooltipTrigger
            class="rounded-md border-2 border-gray-500 p-4 hover:border-blue-500 hover:bg-slate-700"
          >
            <Icon icon="bi:git" class="mx-auto h-16 w-16 md:h-24 md:w-24" />
            <span class="mt-2 block text-center font-bold">Git</span>
          </TooltipTrigger>
        </Tooltip>
      </TooltipProvider>
    </div>
  </div>
</template>
