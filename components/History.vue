<template>
  <div>
    <article
      class="p-8 max-w-lg border-2 rounded-lg m-2 dark:border-cyan-300 light:slate-900"
    >
      <h2 class="category-title">{{ title }}</h2>
      <ul v-for="item in data" :key="item.id">
        <Card :item="item" />
      </ul>
    </article>
  </div>
</template>
<script>
export default {
  props: {
    title: {
      type: String,
      required: true,
    },
    data: {
      type: Array,
      required: true,
    },
  },
};
</script>
<style></style>
