<template>
  <NuxtLayout name="default">
    <h1 class="text-center text-4xl">Resume</h1>

    <div
      class="flex flex-wrap lg:justify-center flex-cols-3 m-auto md:justify-start p-16"
    >
      <History title="Work" :data="history.workHistory" />
      <History title="Education" :data="history.educationHistory" />
      <Skills :data="history.skills" />
    </div>
  </NuxtLayout>
</template>

<style>
.category-title {
  @apply text-2xl font-bold;
}
</style>

<script>
export default {
  data() {
    return {
      history: {
        workHistory: [
          {
            title: "Frontend Developer",
            company: "Freelance",
            location: "Remote",
            date: "2021 - Present",
            description:
              "I am currently working on a freelance project for a client in the UK. I am building a website for a local business using Nuxt.js, Tailwind CSS, and Netlify CMS. I am also using Netlify to host the site and deploy it automatically when changes are made to the CMS.",
          },
          {
            title: "Frontend Developer",
            company: "Freelance",
            location: "Remote",
            date: "2020 - 2021",
            description:
              "I am currently working on a freelance project for a client in the UK. I am building a website for a local business using Nuxt.js, Tailwind CSS, and Netlify CMS. I am also using Netlify to host the site and deploy it automatically when changes are made to the CMS.",
          },
        ],

        educationHistory: [
          {
            title: "Information Technology",
            school: "University of the People",
            location: "Remote",
            date: "2020 - 2022",
            description:
              "Information and techonolgy diploma, with a focus on web development.",
          },
        ],
        skills: [
          {
            title: "HTML",
            level: "90%",
          },
          {
            title: "CSS",
            level: "90%",
          },
          {
            title: "JavaScript",
            level: "80%",
          },
          {
            title: "Vue.js",
            level: "80%",
          },
          {
            title: "Nuxt.js",
            level: "80%",
          },
          {
            title: "Tailwind CSS",
            level: "80%",
          },
        ],
      },
    };
  },
};
</script>
