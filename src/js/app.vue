<template lang="pug">
  <div>
    <Form v-on:nameChange="onNameChange"></Form>
  </div>
</template>

<script>
import Form from './components/form'
export default {
  components: {
    Form
  },
}
</script>

<style lang="scss" scoped>
.container {
  color: green;
}
</style>