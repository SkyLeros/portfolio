<script lang="ts" setup></script>

<template>
  <div class="flex min-h-[70vh] flex-col justify-center py-12 xl:px-0">
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
              Jacqueline Cheers Project
            </h2>
            <!-- Project Description -->
            <h3 class="text-white/60">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit.
              Inventore sed consequuntur error repudiandae numquam deserunt
              quisquam repellat libero asperiores earum nam nobis, culpa ratione
              quam perferendis esse, cupiditate neque quas!
            </h3>
            <!-- Project Stack Icons -->
            <ul class="flex gap-4 text-xl text-white">
              <li>test</li>
              <li>test</li>
              <li>test</li>
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
                    <Button variant="outline" class="w-[20%]"> Hover </Button>
                  </TooltipTrigger>
                  <TooltipContent>
                    <p>Add to library</p>
                  </TooltipContent>
                </Tooltip>
              </TooltipProvider>
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
  <div class="flex flex-col justify-center xl:px-0">
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
              PNWX Web Application
            </h2>
            <!-- Project Description -->
            <h3 class="text-white/60">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit.
              Inventore sed consequuntur error repudiandae numquam deserunt
              quisquam repellat libero asperiores earum nam nobis, culpa ratione
              quam perferendis esse, cupiditate neque quas!
            </h3>
            <!-- Project Stack Icons -->
            <ul class="flex gap-4 text-xl text-white">
              <li>test</li>
              <li>test</li>
              <li>test</li>
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
                    <Button variant="outline" class="w-[20%]"> Hover </Button>
                  </TooltipTrigger>
                  <TooltipContent>
                    <p>Add to library</p>
                  </TooltipContent>
                </Tooltip>
              </TooltipProvider>
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

<style></style>
