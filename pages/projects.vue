<script lang="ts" setup>
import { Icon } from "@iconify/vue";
</script>

<template>
  <!-- First Project -->
  <div
    v-motion-fade
    class="flex min-h-[70vh] flex-col justify-center py-12 xl:px-0"
  >
    <div class="container mx-auto">
      <div class="flex flex-col xl:flex-row xl:gap-6">
        <div
          class="order-2 flex w-full flex-col xl:order-none xl:h-[460px] xl:w-[50%] xl:justify-between"
        >
          <div class="flex flex-col gap-[30px]">
            <!-- Project No.  -->
            <h1
              class="text-outline text-8xl font-extrabold leading-none text-white"
            >
              01
            </h1>
            <!-- Project Category -->
            <h2
              class="group:hover:text-accent text-[42px] font-bold capitalize leading-none text-white transition-all duration-500"
            >
              Jacqueline Cheers System
            </h2>
            <!-- Project Description -->
            <h3 class="text-white/60">
              Jacqueline Cheers System is a sophisticated web-based salon
              management application developed to optimize salon operations. It
              features a comprehensive customer interface for user registration,
              profile management, appointment scheduling, and secure checkout.
              The admin dashboard allows efficient management of service
              appointments, product orders, and detailed reporting, ensuring
              streamlined and effective salon administration. This project
              demonstrates expertise in full-stack web development, user
              experience design, and secure transaction processing.
            </h3>
            <!-- Project Stack Icons -->
            <ul class="flex gap-4 text-xl text-white">
              <Icon icon="material-symbols:php-sharp" class="size-12" />
              <Icon icon="akar-icons:javascript-fill" class="size-12" />
              <Icon icon="simple-icons:mysql" class="size-12" />
              <Icon icon="bi:git" class="size-12" />
            </ul>
            <!-- Border -->
            <div class="border border-white/20"></div>
            <!-- Buttons -->
            <div class="flex items-center gap-4">
              <TooltipProvider :delayDuration="100">
                <Tooltip>
                  <TooltipTrigger
                    as-child
                    class="group flex w-[70px] items-center justify-center rounded-full bg-white/5"
                  >
                    <Button variant="outline" class="w-[20%]"> Visit </Button>
                  </TooltipTrigger>
                </Tooltip>
              </TooltipProvider>
              <NuxtLink
                to="https://github.com/SkyLeros/jacqueline-cheers-system"
                class="mx-3 text-white hover:text-blue-500"
                target="_blank"
                ><Icon
                  icon="mdi:github"
                  class="size-12 gap-6 rounded-full border p-[6px] hover:border-blue-500"
              /></NuxtLink>
            </div>
          </div>
        </div>

        <!-- Second Column -->
        <div class="w-full xl:w-[50%]">
          <div class="mb-12 xl:h-[520px]">
            <div
              class="group relative flex h-[460px] items-center justify-center bg-slate-500"
            >
              <!-- Overlay -->
              <div></div>
              <!-- Image -->
              <img class="relative h-full w-full" src="" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- 2nd Project -->
  <div v-motion-fade class="my-6 flex flex-col justify-center xl:px-0">
    <div class="container mx-auto">
      <div class="flex flex-col xl:flex-row xl:gap-6">
        <div
          class="order-2 flex w-full flex-col xl:order-none xl:h-[460px] xl:w-[50%] xl:justify-between"
        >
          <div class="flex flex-col gap-[30px]">
            <!-- Project No.  -->
            <h1
              class="text-outline text-8xl font-extrabold leading-none text-white"
            >
              02
            </h1>
            <!-- Project Category -->
            <h2
              class="group:hover:text-accent text-[42px] font-bold capitalize leading-none text-white transition-all duration-500"
            >
              Pacific Northwest X-Ray (PNWX) E-commerce Web Appllication
            </h2>
            <!-- Project Description -->
            <h3 class="text-white/60">
              Pacific Northwest X-Ray (PNWX) is a comprehensive web-based
              e-commerce platform designed to enhance user experience and
              streamline online shopping. Developed for a university course on
              Web-Based System Development with my team, the application offers
              a robust user interface for both customers and administrators. Key
              features include customer registration and login, detailed product
              catalogs, shopping cart functionality, and secure checkout with
              OTP validation while the admin dashboard provides extensive
              control over product information and analytical insights through
              visual charts and tables. This project showcases proficiency in
              web development, user experience design, and secure transaction
              processing.
            </h3>
            <!-- Project Stack Icons -->
            <ul class="flex gap-4 text-xl text-white">
              <Icon icon="material-symbols:php-sharp" class="size-12" />
              <Icon icon="akar-icons:javascript-fill" class="size-12" />
              <Icon icon="simple-icons:mysql" class="size-12" />
              <Icon icon="bi:git" class="size-12" />
            </ul>
            <!-- Border -->
            <div class="border border-white/20"></div>
            <!-- Buttons -->
            <div class="flex items-center gap-4">
              <TooltipProvider :delayDuration="100">
                <Tooltip>
                  <TooltipTrigger
                    as-child
                    class="group flex w-[70px] items-center justify-center rounded-full bg-white/5"
                  >
                    <Button variant="outline" class="w-[20%]"> Visit </Button>
                  </TooltipTrigger>
                </Tooltip>
              </TooltipProvider>
              <NuxtLink
                to="https://github.com/SkyLeros/pacific-northwest-x-ray"
                class="text-white hover:text-blue-500"
                target="_blank"
                ><Icon
                  icon="mdi:github"
                  class="mx-3 size-12 gap-6 rounded-full border p-[6px] hover:border-blue-500"
              /></NuxtLink>
            </div>
          </div>
        </div>

        <!-- Second Column -->
        <div class="w-full xl:w-[50%]">
          <div class="mb-12 xl:h-[520px]">
            <div
              class="group relative flex h-[460px] items-center justify-center bg-slate-500"
            >
              <!-- Overlay -->
              <div></div>
              <!-- Image -->
              <img class="relative h-full w-full" src="" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Third Project -->
  <div v-motion-fade class="my-6 flex flex-col justify-center xl:px-0">
    <div class="container mx-auto">
      <div class="flex flex-col xl:flex-row xl:gap-6">
        <div
          class="order-2 flex w-full flex-col xl:order-none xl:h-[460px] xl:w-[50%] xl:justify-between"
        >
          <div class="flex flex-col gap-[30px]">
            <!-- Project No.  -->
            <h1
              class="text-outline text-8xl font-extrabold leading-none text-white"
            >
              03
            </h1>
            <!-- Project Category -->
            <h2
              class="group:hover:text-accent text-[42px] font-bold capitalize leading-none text-white transition-all duration-500"
            >
              Health Diary Application
            </h2>
            <!-- Project Description -->
            <h3 class="text-white/60">
              The Health Diary Application is a comprehensive Java-based
              solution designed for tracking and managing health metrics.
              Developed as part of a university course on Java Programming, this
              application enables users to calculate their Body Mass Index
              (BMI), record health data, and monitor their BMI history over
              time. The app provides a user-friendly interface for logging and
              retrieving health records, facilitating consistent health tracking
              and promoting wellness.
            </h3>
            <!-- Project Stack Icons -->
            <ul class="flex gap-4 text-xl text-white">
              <Icon icon="ri:java-fill" class="size-12" />
            </ul>
            <!-- Border -->
            <div class="border border-white/20"></div>
            <!-- Buttons -->
            <div class="flex items-center gap-4">
              <TooltipProvider :delayDuration="100">
                <Tooltip>
                  <TooltipTrigger
                    as-child
                    class="group flex w-[70px] items-center justify-center rounded-full bg-white/5"
                  >
                    <Button variant="outline" class="w-[20%]"> Visit </Button>
                  </TooltipTrigger>
                </Tooltip>
              </TooltipProvider>
              <NuxtLink
                to="https://github.com/SkyLeros/health-diary-application"
                class="text-white hover:text-blue-500"
                target="_blank"
                ><Icon
                  icon="mdi:github"
                  class="mx-3 size-12 gap-6 rounded-full border p-[6px] hover:border-blue-500"
              /></NuxtLink>
            </div>
          </div>
        </div>

        <!-- Second Column -->
        <div class="w-full xl:w-[50%]">
          <div class="mb-12 xl:h-[520px]">
            <div
              class="group relative flex h-[460px] items-center justify-center bg-slate-500"
            >
              <!-- Overlay -->
              <div></div>
              <!-- Image -->
              <img class="relative h-full w-full" src="" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>