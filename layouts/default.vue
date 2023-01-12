<template>
  <body class="dark:bg-slate-900 dark:text-white">
    <NavBar
      :darkModeHandler="
        () => setColorTheme($colorMode.preference == 'dark' ? 'light' : 'dark')
      "
    />
    <div class="pt-36 h-auto">
      <slot />
    </div>
  </body>
</template>

<script lang="ts">
export default {
  methods: {
    setColorTheme: function (newTheme: Theme) {
      this.$colorMode.preference = newTheme;
    },
  },
};

type Theme = "light" | "dark";
</script>
