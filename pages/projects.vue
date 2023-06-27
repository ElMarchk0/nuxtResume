<template>
  <NuxtLayout name="default">
    <h1 class="text-center text-4xl mb-16">Projects</h1>
    <div
      class="flex flex-wrap justify-between md:justify-center flex-cols-3 m-auto"
    >
      <ul v-for="item in projects" :key="item.id">
        <ProjectCard :item="item" />
      </ul>
    </div>
  </NuxtLayout>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          title: "Beer API",
          desc: "An API the searches for craft beer brewed in Victoria, BC. Built with Nuxt.js, Tailwind, and MongoDB.",
          link: "https://beer-api-v2.vercel.app/",
          repo: "https://github.com/ElMarchk0/beerApiV2",
        },
        {
          title: "Indigenous Perspectives Society Capstone Project",
          desc: "A data collection and reporting web application built for the Indigenous Perspectives Society(IPS) as a part of my diploma at Camosun College. My role in the team was built the API and implement hosting on a local server. The API is built with Django and MySQL",
        },
        {
          title: "Rick Roller",
          desc: "A simple webpage built with vanilla js and css",
          link: "#",
          repo: "https://github.com/ElMarchk0/beerApiV2",
        },
      ],
    };
  },
};
</script>
