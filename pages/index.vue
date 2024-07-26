<script setup lang="ts">
import { Icon } from "@iconify/vue";
</script>

<template>
  <div class="mx-12 my-5 flex flex-col text-white md:flex-row">
    <div class="space-y-5 md:flex-1">
      <h3>Full-stack Developer</h3>
      <h1 class="text-4xl font-bold">
        Hello, I'm <br /><span class="text-blue-500">Than Ye Hong</span>
      </h1>
      <p class="text-lg">Brief description of myself goes here...</p>
      <Button variant="outline" class="my-4">
        <Icon icon="ic:sharp-download" />Download CV
      </Button>
    </div>
    <div class="my-5 flex-1 md:my-0 md:ml-auto">
      <img
        src="~/assets/img/profilepic.jpg"
        alt="Profile Picture"
        class="mx-auto w-full max-w-xs rounded-full md:max-w-sm lg:max-w-md"
      />
    </div>
  </div>
</template>
