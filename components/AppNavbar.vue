<script lang="ts" setup></script>

<template>
  <header v-motion-fade class="relative py-8 text-white xl:py-12">
    <div class="container mx-auto flex items-center justify-between">
      <NuxtLink to="/" class="text-4xl font-extrabold"
        >Ye Hong<span class="text-blue-500">.</span>
      </NuxtLink>
      <div class="hidden items-center gap-10 text-lg xl:flex">
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
      <!-- Mobile Nav Bar -->
      <div class="xl:hidden"><MobileNav /></div>
    </div>
  </header>
</template>
