<template lang="pug">
  li.artist
    h2: a(:href='artist.url' target='_blank') {{artist.name}}
    img(:src="artist.image[2]['#text']")
</template>

<script>
export default {
  name: 'artist',
  props: [ 'artist' ]
}
</script>

<style lang='stylus' scoped>
li.artist

    margin 10px 61px
    width 10%
    max-height 300px
    padding 20px 10px
    border lightcoral thin solid
    box-shadow inset 2px 2px 2px rgba(104,104,104,0.5)
    border-radius 5px
    background-color white

</style>
