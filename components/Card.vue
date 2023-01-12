<template>
  <div class="m-auto p-4">
    <h3 class="font-bold">{{ item.title }}</h3>
    <p class="font-semibold">{{ item.company }}</p>
    <div class="px-2">
      <p class="font-light italic">{{ item.location }}</p>
      <p class="font-light italic">{{ item.date }}</p>
      <ul v-for="subitem in item.description" :key="subitem.id">
        <li>
          <p class="pt-2">{{ subitem }}</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  props: ["item"],
};
</script>
