<template>
  <div>
    <article class="p-16 max-w-prose m-auto">
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
