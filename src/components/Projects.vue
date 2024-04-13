<script setup>
const projects = [
  {
    name: "Food Delivery UI",
    img: "/food_app.png",
    link: "https://github.com/Bilawal-Mehfooz-Malik/simple_food_app",
  },
  {
    name: "Virtual Card",
    img: "/virtual_card.png",
    link: "https://github.com/Bilawal-Mehfooz-Malik/v_card",
  },
  {
    name: "Chat App",
    img: "/chat_app.png",
    link: "https://github.com/Bilawal-Mehfooz-Malik/chat_app",
  },
];
</script>

<template>
  <section class="py-4 lg:py-16 my-4 lg:my-16 border-y-2 border-gray-800">
    <div id="projects" class="px-4 md:px-0">
      <h2
        class="text-2xl lg:text-3xl lg:leading-relaxed font-semibold leading-snug text-gray-900"
      >
        Projects
      </h2>
      <div class="grid projects__grid mt-4">
        <article
          v-for="(project, index) in projects"
          :key="index"
          class="border rounded border-gray-800"
        >
          <a :href="project.link">
            <div class="relative border-b border-gray-800">
              <div class="">
                <img class="rounded-t w-[100%]" :src="project.img" alt="" />
              </div>
            </div>
          </a>
          <header class="px-4 py-2 border-gray-800">
            <h3 class="text-xl">{{ project.name }}</h3>
          </header>
          <!-- <footer class="flex">
            <div class="flex-1 border-r border-gray-800"></div>
            <div class="p-2 w-14">
              <a :href="project.downloadLink">
                <img
                  class="w-[70%] mx-auto"
                  src="/src/assets/download.png"
                  alt=""
                />
              </a>
            </div>
          </footer> -->
        </article>
      </div>
    </div>
  </section>
</template>
<style scoped>
.projects__grid {
  --min-grid-absolute-size: 16rem;
  --max-grid-relative-size: 33%;
  display: grid;
  grid-template-columns: repeat(
    auto-fill,
    minmax(
      max(
        min(var(--min-grid-absolute-size), 100%),
        var(--max-grid-relative-size) - 1rem
      ),
      1fr
    )
  );
  gap: 1rem;
}
</style>
