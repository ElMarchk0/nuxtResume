<template>
  <nav
    class="fixed w-screen bg-white dark:bg-slate-900 px-8 py-8 mx-auto md:flex md:justify-between md:items-center"
  >
    <div class="flex items-center justify-between">
      <h1 class="text-center text-2xl">Peter Charlesworth</h1>

      <div @click="showMenu = !showMenu" class="flex md:hidden">
        <button type="button" class="menu-btn" aria-label="toggle menu">
          <svg
            id="menu-button"
            class="h-6 w-6 cursor-pointer md:hidden block"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"
            />
          </svg>
        </button>
      </div>
    </div>
    <ul
      :class="showMenu ? 'flex' : 'hidden'"
      class="flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0"
    >
      <NuxtLink to="/" class="no-underline hover:text-blue-400">
        About Me
      </NuxtLink>
      <li class="link">
        <NuxtLink to="/projects">Projects</NuxtLink>
      </li>
      <li class="link">
        <NuxtLink to="/resume">Resume</NuxtLink>
      </li>
      <li class="link">
        <font-awesome-icon icon="fa-brands fa-github-square" />
        <NuxtLink class="px-2" to="https://github.com/ElMarchk0"
          >Github</NuxtLink
        >
      </li>
      <li class="link">
        <font-awesome-icon icon="fa-brands fa-linkedin" />
        <NuxtLink
          class="px-2"
          to="https://www.linkedin.com/in/peter-charlesworth-22b866215/"
          >LinkedIn</NuxtLink
        >
      </li>
      <li>
        <Toggle :darkModeHandler="darkModeHandler" />
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  props: {
    darkModeHandler: {
      type: Function,
      required: true,
    },
  },
  data() {
    return {
      showMenu: false,
    };
  },
  methods: {
    toggleNav: function () {
      this.showMenu = !this.showMenu;
    },
  },
};
</script>
<style scoped>
.link {
  @apply md:p-4 py-2 block hover:text-blue-400;
}
.menu-btn {
  @apply text-gray-800 hover:text-gray-400 focus:outline-none focus:text-gray-400;
}
</style>
