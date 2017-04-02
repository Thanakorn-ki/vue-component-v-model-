<template>
  <div id="app">
    <text-box title="Thanakorns" v-model="firstname"></text-box>
    {{firstname}}
  </div>
</template>

<script>
import TextBox from './TextBox.vue'
export default {
  name: 'app',
  data () {
    return {
      firstname: ''
    }
  },
  components: {
    TextBox
  }
}
</script>
