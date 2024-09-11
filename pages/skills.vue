<script lang="ts" setup>
import {
  Tooltip,
  TooltipContent,
  TooltipProvider,
  TooltipTrigger,
} from "@/components/ui/tooltip";
import { Icon } from "@iconify/vue";

interface Skill {
  icon: string;
  name: string;
  description?: string;
}

const skills: Skill[] = [
  { icon: "akar-icons:javascript-fill", name: "Javascript", description: "Versatile programming language for web development" },
  { icon: "akar-icons:typescript-fill", name: "Typescript", description: "Typed superset of JavaScript" },
  { icon: "fa6-brands:vuejs", name: "Vue Js", description: "Progressive JavaScript framework" },
  { icon: "tabler:brand-nuxt", name: "Nuxt Js", description: "Vue.js framework for building web applications" },
  { icon: "material-symbols:php-sharp", name: "PHP", description: "Server-side scripting language" },
  { icon: "simple-icons:laravel", name: "Laravel", description: "PHP web application framework" },
  { icon: "ri:tailwind-css-fill", name: "Tailwind CSS", description: "Utility-first CSS framework" },
  { icon: "devicon-plain:mysql-wordmark", name: "MySQL", description: "Open-source relational database management system" },
  { icon: "simple-icons:sqlite", name: "SQLite", description: "Lightweight, serverless database engine" },
  { icon: "bi:git", name: "Git", description: "Distributed version control system" },
  { icon: "uil:docker", name: "Docker", description: "Platform for developing, shipping, and running applications" },
  { icon: "gg:figma", name: "Figma", description: "Collaborative interface design tool" },
];
</script>

<template>
  <div v-motion-fade class="container mx-auto">
    <div class="mb-5 gap-4 text-center">
      <h1 class="text-4xl font-extrabold text-blue-500 lg:text-5xl">Skills</h1>
    </div>
    <div
      class="mx-4 grid grid-cols-1 gap-6 p-4 text-white sm:mx-6 sm:grid-cols-2 md:mx-10 md:grid-cols-3 lg:mx-20 lg:gap-6"
    >
      <TooltipProvider
        v-for="skill in skills"
        :key="skill.name"
        class="flex items-center justify-center"
        :delayDuration="100"
      >
        <Tooltip>
          <TooltipTrigger
            class="rounded-md border-2 border-gray-500 p-4 hover:border-blue-500 hover:bg-slate-700"
          >
            <Icon
              :icon="skill.icon"
              class="mx-auto h-16 w-16 md:h-24 md:w-24"
            />
            <span class="mt-2 block text-center font-bold">{{ skill.name }}</span>
          </TooltipTrigger>
          <TooltipContent v-if="skill.description">
            <p>{{ skill.description }}</p>
          </TooltipContent>
        </Tooltip>
      </TooltipProvider>
    </div>
  </div>
</template>