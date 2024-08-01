<script setup lang="ts">
import { Icon } from "@iconify/vue";
</script>

<template>
  <div
    v-motion-fade-visible-once
    class="bg-[#1e293b] flex flex-col justify-center py-12 md:mx-4 xl:px-0"
  >
    <div class="container mx-auto h-full">
      <div
        class="flex flex-col items-center justify-between xl:flex-row xl:gap-6"
      >
        <div
          class="order-2 w-full xl:order-none xl:h-[460px] xl:justify-between"
        >
          <div class="gap-[30px] text-center text-white xl:text-left">
            <h3 class="mb-6 text-xl">Full-stack Developer</h3>
            <h1 class="mb-6 text-4xl font-bold xl:text-6xl">
              Hello, I'm <br /><span class="text-blue-500">Than Ye Hong</span>
            </h1>
            <p class="max-width-[500px] mb-9 text-xl text-white/80">
              Brief description of myself goes here....
            </p>
            <div class="flex flex-col items-center gap-4 xl:flex-row">
              <Button
                variant="outline"
                class="flex items-center gap-2 rounded-2xl text-xl uppercase"
              >
                <Icon icon="ic:sharp-download" />Download CV
              </Button>
              <div class="my-4 flex gap-4 xl:mx-8 xl:my-8 xl:mb-8">
                <NuxtLink to="/" class="hover:text-blue-500"
                  ><Icon
                    icon="mdi:linkedin"
                    class="size-12 gap-6 rounded-full border p-[6px] hover:border-blue-500"
                /></NuxtLink>
                <NuxtLink to="/" class="hover:text-blue-500"
                  ><Icon
                    icon="mdi:github"
                    class="size-12 gap-6 rounded-full border p-[6px] hover:border-blue-500"
                /></NuxtLink>
              </div>
            </div>
          </div>
        </div>

        <div class="relative h-full w-full">
          <div class="mb-12 xl:h-[520px]">
            <div class="group relative flex items-center justify-center">
              <img
                src="~/assets/img/profilepic.jpg"
                alt="Profile Picture"
                class="w-full max-w-xs rounded-full object-contain md:max-w-sm lg:max-w-md"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- <div class="min-h-[80vh] flex flex-col justify-center py-12 xl:px-0">
    <div class="container mx-auto">
      <div class="flex flex-col xl:flex-row xl:gap-6">
        <div class="w-full xl:w-[50%] xl:h-[460px] flex flex-col xl:justify-between order-2 xl:order-none"><h1 class="text-4xl font-extrabold text-white">01</h1>1</div>
        
        <div class="w-full xl:w-[50%]">text</div>
      </div>
    </div>
  </div> -->

  <!-- <div class="mx-12 my-5 flex flex-col text-white md:flex-row">
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
  </div> -->
</template>
