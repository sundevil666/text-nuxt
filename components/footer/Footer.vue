<template lang="pug">
  footer.footer
    .container
      .footer__copy
        .footer__item Beach Surfing
        div Copyright © 2018 All Rights Reserved.
      .footer__design Designed by  <span>Rikon Rahman</span>
</template>

<script>
export default {
name: "Footer"
}
</script>

<style lang="sass">
  .footer .container
    border-top: 1px solid #f2ede7
    display: flex
    justify-content: space-between
    align-items: center
    padding-top: 45px
    padding-bottom: 40px
    font-size: 14px
    font-family: "Avenir"
    color: #9f9f9f

    .footer__item
      font-family: 'Playfair Display'
      font-size: 24px
      color: #000

    .footer__design span
      color: #000

</style>
