<template lang="html">
  <div class="">
    <label :title="title">{{title}}</label>
    <label >{{value}}</label>
    <input ref="inputs" v-bind:value="value" v-on:input="updateValue()">
  </div>
</template>

<script>
export default {
  props: ['title', 'value'],
  methods: {
    updateValue () {
      this.$emit('input', `${this.$refs.inputs.value}`)
    }
  }
}
</script>

<style lang="css">
</style>
