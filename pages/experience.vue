<script lang="ts" setup>
import Timeline from "primevue/timeline";
import Card from "primevue/card";

const events = ref([
  {
    company: "Sarawak Information Systems (SAINS)",
    position: "UX Designer Intern",
    date: "2023 Feb - 2023 Aug",
    color: "#3b82f6",
    content:
      "• Leveraged internal design documentation to ensure consistency and adherence to standards in website layouts and interfaces. \n• Applied AI tools to speed up the design process significantly reducing time and increasing efficiency. \n• Utilized Evolus Pencil Project to create professional mockups, enhancing design quality and stakeholder communication.",
  },
  {
    company: "Beacon Homestay",
    position: "Hospitality Assistant",
    date: "2020 Feb - 2020 Mar",
    color: "#3b82f6",
    content:
      "• Maintained cleanliness and organization of hostel rooms and common areas, ensuring a welcoming and hygienic environment for guests. \n• Provided good customer service by taking orders, serving dishes, and managing the cashier, enhancing the overall guest experience. \n• Promoted and advertised the homestay through various channels, successfully increasing bookings and improving occupancy rates.",
  },
  {
    company: "CS Mart",
    position: "Courtesy Clerk",
    date: "2018 Jan - 2018 Mar",
    color: "#3b82f6",
    content:
      "• Assisted customers with bagging groceries and carrying items to their vehicles, ensuring a pleasant shopping experience. \n• Helped restock shelves and maintain product displays, contributing to an organized and visually appealing store layout. \n• Supported cashiers by managing the flow of customers and reducing wait times at checkout.",
  },
]);
</script>

<template>
  <div v-motion-fade class="card">
    <div class="mx-auto xl:container">
      <Timeline :value="events" class="customized-timeline text-white">
        <template #marker="slotProps">
          <span
            class="h-8 w-8 rounded-full"
            :style="{ backgroundColor: slotProps.item.color }"
          >
          </span>
        </template>
        <template #content="slotProps">
          <Card class="mb-8 mt-4">
            <template #title>
              <span class="text-2xl text-green-400"
                >{{ slotProps.item.company }}<br />
              </span>
              <span class="text-white/90">
                {{ slotProps.item.position }}
              </span>
            </template>
            <template #subtitle>
              {{ slotProps.item.date }}
            </template>
            <template #content>
              <ul>
                <li
                  v-html="slotProps.item.content.replace(/\n/g, '<br><br>')"
                ></li>
              </ul>
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
