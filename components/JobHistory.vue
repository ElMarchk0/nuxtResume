<template>
  <div>
    <article class="p-8 max-w-3xl m-auto">
      <h2>Work History</h2>
      <ul v-for="job in jobs" :key="job.id">
        <JobCard :item="job" />
      </ul>
    </article>
  </div>
</template>
<script>
export default {
  data() {
    return {
      jobs: [
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
    };
  },
};
</script>
