<template lang="pug">
    v-toolbar(height="100px" dark)
      v-container
        v-toolbar-items.justify-center
          v-btn.px-6.py-3.mr-6.btn-style.blue-grey--text.text--lighten-5 О себе
          v-btn.px-6.py-3.mr-6.btn-style.blue-grey--text.text--lighten-5 Опыт работы
          v-btn.px-6.py-3.btn-style.blue-grey--text.text--lighten-5 Контакты

</template>

<script>
  export default {
      name: "app-header",
  }
</script>

<style lang="scss">

  .v-toolbar__items > button.btn-style {
    border-radius: 38px;
    box-shadow: -13px 13px 26px rgba(14, 14, 14, 0.2), 13px -13px 26px rgba(14, 14, 14, 0.2), -13px -13px 26px rgba(54, 54, 54, 0.9), 13px 13px 33px rgba(14, 14, 14, 0.9), inset 1px 1px 2px rgba(54, 54, 54, 0.3), inset -1px -1px 2px rgba(14, 14, 14, 0.5);
  }

</style>
