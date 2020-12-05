<template lang="pug">
  .container-fluid
    .container
      Headers
      Nuxt
    Footer
</template>

<script>
import Headers from "~/components/header/Header";
import Footer from "~/components/footer/Footer";
export default {
  name: 'default',
  components: {
    Headers,
    Footer
  }
}
</script>
<style lang="sass">

  .container
    width: 100%
    max-width: 1490px
    padding: 0 15px
    box-sizing: border-box
    margin: 0 auto
</style>
