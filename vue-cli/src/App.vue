<template>
  <div>
    <app-header 
    v-bind:propsdata="str"
    v-on:renew="renewStr"></app-header>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'

export default {
  data: function() {
    return {
      str: 'Hello world'
    }
  },
  methods: {
      renewStr: function() {
        this.str = 'whole new world';
    }
  },
  components: {
    'app-header': AppHeader
  }
}
</script>

<style>

</style>