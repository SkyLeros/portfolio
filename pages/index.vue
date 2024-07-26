<script setup lang="ts">
import { Icon } from "@iconify/vue";
</script>

<template>
  <div class="flex min-h-[80vh] flex-col justify-center py-12 xl:px-0">
   <div class="container mx-auto"> 
      <div class="flex flex-col xl:flex-row xl:gap-6">
        <div
          class="order-2 flex w-full flex-col xl:order-none xl:h-[460px] xl:w-[50%] xl:justify-between"
        >
          <div class="flex flex-col gap-[30px] text-white">
            <h3 class="text-4xl">Full-stack Developer</h3>
            <h1 class="text-6xl font-bold">
              Hello, I'm <span class="text-blue-500">Than Ye Hong</span>
            </h1>
            <p class="text-xl">Brief description of myself goes here...</p>
            <Button variant="outline" class="mx-auto">
              <Icon icon="ic:sharp-download" />Download CV
            </Button>
          </div>
        </div>

        <div class="w-full xl:w-[50%]">
          <div class="mb-12 xl:h-[520px]">
            <div class="group relative flex items-center justify-center">
              <img
                src="~/assets/img/profilepic.jpg"
                alt="Profile Picture"
                class="mx-auto w-full max-w-xs rounded-full md:max-w-sm lg:max-w-md"
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
