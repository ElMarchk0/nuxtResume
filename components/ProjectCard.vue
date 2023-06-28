<template>
  <div
    class="flex flex-col items-center p-8 m-4 max-w-md border-2 rounded-lg dark:border-cyan-300 light:slate-900"
  >
    <h1 class="text-2xl text-center font-bold mt-2">{{ item.title }}</h1>
    <p class="text-gray-700 font-light text-justify mt-3 dark:text-slate-100">
      {{ item.desc }}
    </p>

    <div class="flex flex-col items-center mt-5">
      <a
        v-if="item.link"
        :href="item.link"
        target="_blank"
        rel="noopener noreferrer"
        class="text-sm text-blue-400"
      >
        View Project
      </a>

      <a
        v-if="item.repo"
        :href="item.repo"
        target="_blank"
        rel="noopener noreferrer"
        class="text-sm text-blue-400"
      >
        View Repo
      </a>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  props: ["item"],
};
</script>
