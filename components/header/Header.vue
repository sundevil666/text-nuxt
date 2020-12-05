<template lang="pug">
  header.header
    Logo
    Navbar
</template>

<script>
import Logo from "~/components/header/Logo"
import Navbar from "~/components/header/Navbar";

export default {
  name: 'Header',
  components: {
    Logo,
    Navbar,
  }
}
</script>
<style lang="sass">
  .header
    margin-top: 90px
    display: flex
    justify-content: space-between
</style>
