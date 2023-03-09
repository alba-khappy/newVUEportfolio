<template lang="pug">
  v-app(dark)
    app-header.d-flex.justify-center.align-center
    nuxt
    app-footer

</template>

<style>

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}

</style>

<script>
  import AppHeader from "../components/AppHeader";
  import AppFooter from "../components/AppFooter";

  export default {
      components: {AppHeader, AppFooter}
  }
</script>
