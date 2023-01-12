<template>
  <NuxtLayout name="default">
    <h1 class="text-center text-4xl mb-16">Projects</h1>
    <div
      class="flex flex-wrap justify-between md:justify-center flex-cols-3 m-auto"
    >
      <ul v-for="item in projects" :key="item.id">
        <ProjectCard :item="item" />
      </ul>
    </div>
  </NuxtLayout>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          title: "Beer API",
          desc: "An SPA and API the searches for craft beer brewed in Victoria, BC",
          link: "#",
          repo: "#",
          img: "https://imgs.search.brave.com/3e4Uc7wYfNVqQ3DiU4yAM-QBdQMWimfTNWa6irVrZfA/rs:fit:512:512:1/g:ce/aHR0cHM6Ly9saDMu/Z29vZ2xldXNlcmNv/bnRlbnQuY29tL3lF/RHRqLVY1eFMzS0VS/NGZsZU9MVGVDOGVG/TGN1Q2FsbWIxZ3VT/LWVpMnpRS0Ntbkxx/MXBLdmktY2R3MDRD/aHozaE9u",
        },
        {
          title: "Beer API",
          desc: "An SPA and API the searches for craft beer brewed in Victoria, BC",
          link: "#",
          repo: "#",
          img: "https://imgs.search.brave.com/3e4Uc7wYfNVqQ3DiU4yAM-QBdQMWimfTNWa6irVrZfA/rs:fit:512:512:1/g:ce/aHR0cHM6Ly9saDMu/Z29vZ2xldXNlcmNv/bnRlbnQuY29tL3lF/RHRqLVY1eFMzS0VS/NGZsZU9MVGVDOGVG/TGN1Q2FsbWIxZ3VT/LWVpMnpRS0Ntbkxx/MXBLdmktY2R3MDRD/aHozaE9u",
        },
        {
          title: "Beer API",
          desc: "An SPA and API the searches for craft beer brewed in Victoria, BC",
          link: "#",
          repo: "#",
          img: "https://imgs.search.brave.com/3e4Uc7wYfNVqQ3DiU4yAM-QBdQMWimfTNWa6irVrZfA/rs:fit:512:512:1/g:ce/aHR0cHM6Ly9saDMu/Z29vZ2xldXNlcmNv/bnRlbnQuY29tL3lF/RHRqLVY1eFMzS0VS/NGZsZU9MVGVDOGVG/TGN1Q2FsbWIxZ3VT/LWVpMnpRS0Ntbkxx/MXBLdmktY2R3MDRD/aHozaE9u",
        },
      ],
    };
  },
};
</script>
