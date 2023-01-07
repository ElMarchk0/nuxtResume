<template>
  <div>
    <article class="p-8 max-w-3xl m-auto">
      <h2>Education</h2>
      <ul v-for="item in educationHistory" :key="item.id">
        <EducationCard :item="item" />
      </ul>
    </article>
  </div>
</template>
<script>
export default {
  data() {
    return {
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
    };
  },
};
</script>
