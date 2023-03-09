<template lang="pug">
    v-footer(dark height="100px")
      v-container
        v-spacer
        div &copy; А. С. Хапилина, {{ new Date().getFullYear() }}

</template>

<script>
    export default {
        name: "app-footer",
    }
</script>

<style>
</style>
