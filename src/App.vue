<template>
  <div id="app">
    <rs-header />

    <router-view />

    <rs-footer />
  </div>
</template>

<script>
  import RsHeader from '@/components/layout/Header.vue'
  import RsFooter from '@/components/layout/Footer.vue'

  export default {
    components: { RsHeader, RsFooter }
  }
</script>

<style lang="scss">
  @import "./scss/main.scss";
</style>
