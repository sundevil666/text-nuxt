<template lang="pug">
  nav
    ul.flex
      li(v-for="(item, index) in nav", :key="index")
        a(:href="item.url") {{ item.title }}
</template>

<script>
export default {
  name: "Navbar",
  data: () => ({
    nav: [
      {url: '#', title: 'Home'},
      {url: '#', title: 'About'},
      {url: '#', title: 'Blog'},
      {url: '#', title: 'Contact'},
    ]
  }),
}
</script>

<style lang="sass">
  nav
    min-width: 400px
  nav ul
    justify-content: space-between
    align-items: flex-end
    height: 100%
  nav a
    font-family: avenir-medium
    color: #aaaaaa
    transition: color .5s
    font-size: 15px
    text-transform: uppercase

    &:hover, &.active
      color: #111111
</style>
