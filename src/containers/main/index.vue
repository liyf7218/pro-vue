<template>
  <section class="main">
    {{msg}}
  </section>
</template>

<script>
export default {
  name: 'iMain',
  data () {
    return {
      msg: 'this is the iMain.'
    }
  }
}
</script>

<style scoped>
.main {
    min-height: 600px;
}
</style>
