<script lang="ts" setup></script>

<template>
  <div class="mb-16 bg-slate-800">
    <nav class="flex items-center justify-between p-10 text-white">
      <NuxtLink to="/" class="mx-2 text-2xl font-semibold"
        >Ye Hong <span class="text-blue-500">.</span>
      </NuxtLink>
      <div class="flex gap-10 text-lg">
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
      </div>
    </nav>
  </div>
</template>
