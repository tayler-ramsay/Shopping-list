<template>
  <div>
    <em>Change the list color</em>
    <input v-model="bgColor" placeholder="Change Color">
  </div>
</template>

<script>
export default {
  props: ['value'],
  methods: {
    onInput (e) {
      this.$emit('input', e.target.value)
    }
  }
}
</script>

<style scoped>
input {
  margin-top: 2em;
}
</style>