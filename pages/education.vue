<script lang="ts" setup>
import Timeline from "primevue/timeline";
import Card from "primevue/card";

const events = ref([
  {
    company: "Bachelor of Software Engineering with Honours",
    position: "University of Malaysia, Sarawak (UNIMAS)",
    date: "2023 Feb - 2023 Aug",
    color: "#3b82f6",
    content:
      "• Presented research findings on my final year project titled 'Enhancing Digital Food Menus for Older Adults: A TAM-Based UI/UX Design Evaluation' at my university symposium, demonstrating effective communication and presentation skills. \n• Gained hands-on experience through internships and practical lab sessions, applying theoretical knowledge to real-world software development challenges and gaining valuable industry insights. \n• Utilized industry-standard tools and technologies such as C, C++, Java, PHP and SQL in various projects and lab sessions, ensuring proficiency in modern software development practices. \n• Collaborated on multi-disciplinary team projects, enhancing teamwork, communication, and leadership abilities while delivering high-quality software solutions.",
  },
  {
    company: "Sijil Tinggi Persekolahan Malaysia (STPM)",
    position: "SMK Batu Lintang",
    date: "2018 Jun - 2019 Nov",
    color: "#3b82f6",
    content:
      "• Achieved high academic performance with a CGPA of 3.58/4,00, consistently ranking in the top percentile of the class. \n• Actively participated in co-curricular activities, including the Lions International Club and International Red Cross and Red Crescent Club, developing leadership and critical thinking abilities. \n• Awarded for excellence in Kangaroo Math Competition (KMC), reflecting a broad understanding and passion in mathematics.",
  },
  {
    company: "Sijil Pelajaran Malaysia (SPM)",
    position: "SMK Jalan Arang",
    date: "2016 Jan - 2017 Oct",
    color: "#3b82f6",
    content:
      "• Graduated with excellent results, achieving total grades of 7As \n• Received awards for academic excellence, including Best Student in Mathematics and Science. \n• Maintained a consistent academic record throughout my student years, with a focus on continuous improvement and excellence.",
  },
]);
</script>

<template>
  <div v-motion-fade class="card">
    <div class="mx-auto xl:container">
      <div class="mb-5 gap-4 text-center">
        <h1 class="text-4xl lg:text-5xl font-extrabold text-blue-500">Education</h1>
      </div>
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
