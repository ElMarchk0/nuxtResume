<template>
  <div>
    <h2>{{ item.title }}</h2>
    <p>{{ item.company }}</p>
    <p>{{ item.location }}</p>
    <p>{{ item.date }}</p>
    <p>{{ item.description }}</p>
  </div>
</template>

<script>
export default {
  // pass props from parent component
  props: ["item"],
};
</script>
