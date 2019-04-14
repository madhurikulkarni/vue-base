<template>
  <div id="app">
    <RegistrationForm msg="Registration Form"/>
  </div>
</template>

<script>
import RegistrationForm from './components/RegistrationForm.vue'

export default {
  name: 'app',
  components: {
    RegistrationForm
  }
}
</script>
<style>
@import '../src/assets/css/bootstrap-grid.min.css';
</style>