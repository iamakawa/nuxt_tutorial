<template>
  <div class="container">
    <img
      src="https://vueschool.io/img/favicons/apple-touch-icon.png"
      alt="the logo"
    />
    <div>
      <logo />
      <h1 class="title">
        nuxt_tutorial
      </h1>
      <h2 class="subtitle">
        My exceptional Nuxt.js project
      </h2>
      <div class="links">
        <a href="https://nuxtjs.org/" target="_blank" class="button--green">
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
  components: {
    Logo
  }
};
</script>

<style></style>
