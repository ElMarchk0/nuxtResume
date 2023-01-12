<template>
  <div>
    <article class="p-8 sm:p-16 max-w-3xl m-auto">
      <h2 class="category-title">Skills</h2>
      <div class="flex flex-col p-4">
        <ul v-for="item in data" :key="item.id">
          <li>
            {{ `${item.title} ` }}
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
