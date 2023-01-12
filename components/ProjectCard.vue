<template>
  <div class="flex flex-col justify-center items-center p-6">
    <h1 class="text-2xl font-bold mt-2">{{ item.title }}</h1>
    <img
      :src="item.img"
      alt="project image"
      class="w-40 h-40 m-4 rounded-full"
    />
    <p class="text-gray-700 font-light text-center mt-3 dark:text-slate-100">
      {{ item.desc }}
    </p>
  </div>
  <div class="flex flex-col justify-center items-center mt-5">
    <a
      :href="item.link"
      target="_blank"
      rel="noopener noreferrer"
      class="text-sm text-blue-400"
    >
      View Project
    </a>
    <a
      :href="item.repo"
      target="_blank"
      rel="noopener noreferrer"
      class="text-sm md:text-blue-400"
    >
      View Repo
    </a>
  </div>
</template>

<script lang="ts">
export default {
  props: ["item"],
};
</script>
