<script lang="ts" setup>
import Timeline from "primevue/timeline";
import Card from "primevue/card";

const events = ref([
  {
    status: "Internship at SAINS",
    date: "2023 Feb - 2023 Aug",
    icon: "pi pi-shopping-cart",
    color: "#3b82f6",
    image: "game-controller.jpg",
    content:
      "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Inventore sed consequuntur error repudiandae numquam deserunt quisquam repellat libero asperiores earum nam nobis, culpa ratione quam perferendis esse, cupiditate neque quas!",
  },
  {
    status: "Homestay Assistant",
    date: "2020 Feb - 2020 Mar",
    icon: "pi pi-cog",
    color: "#3b82f6",
    content:
      "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Inventore sed consequuntur error repudiandae numquam deserunt quisquam repellat libero asperiores earum nam nobis, culpa ratione quam perferendis esse, cupiditate neque quas!",
  },
  {
    status: "Supermarket Assistant",
    date: "2018 Jan - 2018 March",
    icon: "pi pi-shopping-cart",
    color: "#3b82f6",
    content:
      "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Inventore sed consequuntur error repudiandae numquam deserunt quisquam repellat libero asperiores earum nam nobis, culpa ratione quam perferendis esse, cupiditate neque quas!",
  },
]);
</script>

<template>
  <div class="card">
    <div class="container mx-auto">
      <Timeline :value="events" class="customized-timeline text-white">
        <template #marker="slotProps">
          <span
            class="flex h-8 w-8 items-center justify-center rounded-full text-white shadow-sm"
            :style="{ backgroundColor: slotProps.item.color }"
          >
            <i :class="slotProps.item.icon"></i>
          </span>
        </template>
        <template #content="slotProps">
          <Card class="mt-4 bg-slate-700">
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
    .p-card-body {
      background-color: #283242;
      border-radius: 0.5em;
    }
  }
}
</style>
