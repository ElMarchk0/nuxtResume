<template>
  <NuxtLayout name="default">
    <h1 class="text-center text-4xl mb-16">Projects</h1>
    <div
      class="flex justify-evenly px-2 justify-items-start place-items-center flex-col-3 flex-wrap ]"
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
          title: "The Victoria Craft Beer API",
          desc: "An API that searches for craft beer brewed in Victoria, BC. Built with Nuxt.js, Tailwind, and MongoDB.",
          link: "https://beer-api-v2.vercel.app/",
          repo: "https://github.com/ElMarchk0/beerApiV2",
        },
        {
          title: "Indigenous Perspectives Society Capstone Project",
          desc: "A Trello data collection and reporting web application built for the Indigenous Perspectives Society(IPS) as a part of my diploma at Camosun College. My role in the team was built the API and implement hosting on a local server. The API is built with Django and MySQL",
          link: "https://capstone.camosun.bc.ca/cosc/2023/teams/teamm",
        },
        {
          title: "Rick Roller",
          desc: "A tribute to the Rickroll. A simple webpage built with vanilla HTML and vanilla CSS. The design concept is based on CD jewel cases from the 1980s. ",
          link: "https://rickroller-gy7y48eld-elmarchk0.vercel.app/",
          repo: "https://github.com/ElMarchk0/rickroller",
        },
        {
          title: "React TypeScript Store Front",
          desc: "An E-Commerce built with TypeScript, React, and ChakraUI. Uses the fake store api for the products.",
          link: "https://chakra-ui-demo-navy.vercel.app/",
          repo: "https://github.com/ElMarchk0/chakraUI_demo",
        },
        {
          title: "Django E-Commerce API",
          desc: "An API built with Django and Django Rest Framework. Allows the user to create, read, update, and delete objects in a database. Uses SQLite for the database.",
          repo: "https://github.com/ElMarchk0/shopify_crud",
        },
        {
          title: "This Portfolio Site",
          desc: "This site is built with Nuxt3 and TailwindCSS.",
          repo: "https://github.com/ElMarchk0/pcresume",
        },
      ],
    };
  },
};
</script>
