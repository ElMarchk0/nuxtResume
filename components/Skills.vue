<template>
  <div>
    <article
      class="p-8 m-2 max-w-lg border-2 rounded-lg dark:border-cyan-300 light:slate-900"
    >
      <h2 class="category-title">Skills</h2>
      <div class="flex flex-col p-4">
        <ul v-for="item in data" :key="item.id">
          <li>
            <h3 class="font-bold">{{ item.title }}</h3>
            <p class="font-italic font-light">{{ item.description }}</p>
          </li>
        </ul>
      </div>
    </article>
  </div>
</template>
<script>
export default {
  props: {
    data: {
      type: Array,
      required: true,
    },
  },
};
</script>
