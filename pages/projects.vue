<script lang="ts" setup>
import { Icon } from "@iconify/vue";
import {
  Carousel,
  CarouselContent,
  CarouselItem,
  CarouselNext,
  CarouselPrevious,
} from "@/components/ui/carousel";
import { Card, CardContent } from "@/components/ui/card";

interface Project {
  id: number;
  title: string;
  description: string;
  stack: string[];
  repoUrl: string;
  imageSrc: string;
}

const projects: Project[] = [
  {
    id: 1,
    title: "Jacqueline Cheers System",
    description:
      "Jacqueline Cheers System is a sophisticated web-based salon management application developed to optimize salon operations. It features a comprehensive customer interface for user registration, profile management, appointment scheduling, and secure checkout. The admin dashboard allows efficient management of service appointments, product orders, and detailed reporting, ensuring streamlined and effective salon administration. This project demonstrates expertise in full-stack web development, user experience design, and secure transaction processing.",
    stack: [
      "material-symbols:php-sharp",
      "akar-icons:javascript-fill",
      "simple-icons:mysql",
      "bi:git",
    ],
    repoUrl: "https://github.com/SkyLeros/jacqueline-cheers-system",
    imageSrc: "jcs/homepage.png",
  },
  {
    id: 2,
    title: "Pacific Northwest X-Ray (PNWX) E-commerce Web Application",
    description:
      "Pacific Northwest X-Ray (PNWX) is a comprehensive web-based e-commerce platform designed to enhance user experience and streamline online shopping. Developed for a university course on Web-Based System Development with my team, the application offers a robust user interface for both customers and administrators. Key features include customer registration and login, detailed product catalogs, shopping cart functionality, and secure checkout with OTP validation while the admin dashboard provides extensive control over product information and analytical insights through visual charts and tables. This project showcases proficiency in web development, user experience design, and secure transaction processing.",
    stack: [
      "material-symbols:php-sharp",
      "akar-icons:javascript-fill",
      "simple-icons:mysql",
      "bi:git",
    ],
    repoUrl: "https://github.com/SkyLeros/pacific-northwest-x-ray",
    imageSrc: "pnwx/pnwx-homepage.png",
  },
  {
    id: 3,
    title: "Health Diary Application",
    description:
      "Health Diary Application is a comprehensive Java-based solution designed for tracking and managing health metrics. Developed as part of a university course on Java Programming, this application enables users to calculate their Body Mass Index (BMI), record health data, and monitor their BMI history over time. The app provides a user-friendly interface for logging and retrieving health records, facilitating consistent health tracking and promoting wellness.",
    stack: ["ri:java-fill"],
    repoUrl: "https://github.com/SkyLeros/health-diary-application",
    imageSrc: "/hda/hda-main.png",
  },
];
</script>

<template>
  <div class="flex min-h-[70vh] flex-col justify-center gap-6 xl:px-0">
    <div
      v-motion-fade
      class="flex min-h-[70vh] flex-col justify-center xl:px-0"
    >
      <div class="container mx-auto">
        <div class="mb-6 gap-4 text-center">
          <h1 class="text-4xl font-extrabold text-blue-500 lg:text-5xl">
            Projects
          </h1>
        </div>
        <div
          v-for="(project, index) in projects"
          :key="project.id"
          :class="{ 'my-10': index > 0 }"
          class="flex flex-col xl:flex-row xl:gap-6"
        >
          <div
            class="order-2 flex w-full flex-col xl:order-none xl:h-[460px] xl:w-[50%] xl:justify-between"
          >
            <div class="flex flex-col gap-[30px]">
              <h1
                class="text-outline text-8xl font-extrabold leading-none text-blue-500"
              >
                {{ String(project.id).padStart(2, "0") }}
              </h1>
              <h2
                class="group:hover:text-accent text-[42px] font-bold capitalize leading-none text-white transition-all duration-500"
              >
                {{ project.title }}
              </h2>
              <h3 class="text-white/60">
                {{ project.description }}
              </h3>
              <ul class="flex gap-4 text-xl text-white">
                <Icon
                  v-for="icon in project.stack"
                  :key="icon"
                  :icon="icon"
                  class="size-12"
                />
              </ul>
              <div class="border border-white/20"></div>
              <div class="flex items-center gap-4">
                <TooltipProvider :delayDuration="100">
                  <Tooltip>
                    <TooltipTrigger
                      as-child
                      class="group flex items-center justify-center rounded-full bg-white/5"
                    >
                      <NuxtLink :to="project.repoUrl" target="_blank">
                        <Button
                          variant="outline"
                          class="flex items-center gap-2 rounded-2xl text-xl"
                        >
                          <Icon icon="mdi:github" />Visit Repository</Button
                        >
                      </NuxtLink>
                    </TooltipTrigger>
                  </Tooltip>
                </TooltipProvider>
              </div>
            </div>
          </div>

          <div class="w-full xl:w-[50%]">
            <div
              :class="{
                'xl:h-[620px] xl:py-10': index === 0,
                'xl:h-[720px] xl:py-[120px]': index === 1,
                'xl:h-[520px]': index === 2,
              }"
              class="mb-12"
            >
              <div
                class="group relative flex h-[460px] items-center justify-center"
              >
                <div
                  class="absolute bottom-0 top-0 z-10 h-full w-full bg-black/10"
                ></div>
                <div class="relative h-full w-full">
                  <img
                    class="h-full w-full object-fill"
                    :src="project.imageSrc"
                    :alt="project.title"
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
