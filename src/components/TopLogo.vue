<template>

  <v-avatar
     :size="logoSize"
     :tile="true"
     class="wgu-top-logo"
    >
    <img :src="logoSrc" alt="App Logo">
  </v-avatar>

</template>

<script>

export default {
  name: 'wgu-top-logo',
  data () {
    return {
      logoSrc: this.$appConfig.logo,
      logoSize: this.$appConfig.logoSize
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

  .wgu-top-logo {
    position: absolute;
    z-index: 1000;
    border: 2px solid white;
  }

</style>
