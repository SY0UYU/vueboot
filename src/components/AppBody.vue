<template>
  <div id="temp1">
    <blockquote id="temp2">
      This is a block-quote!
    </blockquote>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'AppBody'
}
</script>

<style scoped>
#temp2 {
  border-left: .25rem solid dodgerblue;
  padding-left: .25rem;
}
</style>
