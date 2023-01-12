<template>
  <div class="m-auto p-4">
    <h3 class="font-bold">{{ item.title }}</h3>
    <p class="font-semibold">{{ item.company }}</p>
    <p class="font-semibold">{{ item.location }}</p>
    <p class="font-semibold">{{ item.date }}</p>
    <p>{{ item.description }}</p>
  </div>
</template>

<script>
export default {
  // pass props from parent component
  props: ["item"],
};
</script>
