<script lang="ts" setup></script>

<template>
  <div class="bg-slate-800 mb-16">
    <nav class="flex items-center justify-between p-10 text-white">
      <NuxtLink to="/" class="mx-2 text-2xl font-semibold"
        >Than Ye Hong <span class="text-blue-500">.</span>
      </NuxtLink>
      <div class="flex gap-10 text-lg">
        <NuxtLink to="/education" class="hover:text-blue-500 hover:border-b-2 border-blue-500">Education</NuxtLink>
        <NuxtLink to="/skills" class="hover:text-blue-500 hover:border-b-2 border-blue-500">Skills</NuxtLink>
        <NuxtLink to="/projects" class="hover:text-blue-500 hover:border-b-2 border-blue-500">Projects</NuxtLink>
      </div>
    </nav>
  </div>
</template>
