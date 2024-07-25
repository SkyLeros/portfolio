<script lang="ts" setup>
import Timeline from "primevue/timeline";
import Card from "primevue/card";

const events = ref([
  {
    status: "Bachelor's Degree of Computer Science (Software Engineering)",
    date: "2020 Oct - 2024 Nov",
    icon: "pi pi-shopping-cart",
    color: "#3b82f6",
    image: "game-controller.jpg",
    content: "test",
  },
  {
    status: "Sijil Tinggi Persekolahan Malaysia (STPM)",
    date: "2018 Jun - 2019 Nov",
    icon: "pi pi-cog",
    color: "#3b82f6",
    content: "test",
  },
  {
    status: "Sijil Pelajaran Malaysia (SPM)",
    date: "2016 Jan - 2017 Oct",
    icon: "pi pi-shopping-cart",
    color: "#3b82f6",
    content: "test",
  },
]);
</script>

<template>
  <div class="card">
    <Timeline :value="events" class="customized-timeline mx-10 text-white">
      <template #marker="slotProps">
        <span
          class="flex h-8 w-8 items-center justify-center rounded-full text-white  shadow-sm"
          :style="{ backgroundColor: slotProps.item.color }"
        >
          <i :class="slotProps.item.icon"></i>
        </span>
      </template>
      <template #content="slotProps">
        <Card class="mt-4">
          <template #title>
            {{ slotProps.item.status }}
          </template>
          <template #subtitle class="bg-purple-700">
            {{ slotProps.item.date }}
          </template>
          <template #content>
            <p>
              {{ slotProps.item.content }}
            </p>
            <Button label="Read more" text></Button>
          </template>
        </Card>
      </template>
    </Timeline>
  </div>
</template>

<style lang="scss" scoped>
@media screen {
  ::v-deep(.customized-timeline) {
    .p-timeline-event:nth-child(even) {
      flex-direction: row;

      .p-timeline-event-content {
        text-align: left;
      }
    }

    .p-timeline-event-opposite {
      flex: 0;
    }
  }
}
</style>
