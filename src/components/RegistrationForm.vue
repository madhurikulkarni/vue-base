<template>

 <div class="container">
  <div class="col-md-8 offset-md-2 col-12">
  <div class="hello">
    <h1  class="centered">{{ msg }}</h1>
        <div class="mod_article">
        <form class="formbody" @submit.prevent="handleClick">
            <div class="widget-text">
                <label for="username">Username</label>
                <input type="text" id="username" v-model="username" class="text" value="" required>
            </div>
            <div class="widget-text">
                <label for="password">Password</label>
                <input type="password" id="password" v-model="password" class="text" value="" required>
            </div>
            <button id="submitButton">Submit</button>
        </form>
        <div class="credits">
            <h3 class="centered">Credits</h3>
            <ul>
              <li>https://alligator.io/vuejs/vue-form-handling/</li>
            </ul>
        </div>
    </div>
    </div>
</div>
  </div>
</template>

<script>

export default {
  name: 'RegistrationForm',
  props: {
    msg: String
  },
  data() {
    return {
      username: null,
      password:null
    }
  },
  methods: {
   handleClick(event){
      alert('The username is:::' + this.username  + ' and the password is:::' + this.password);
      event.target.reset();
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped >
@import '../../src/assets/css/main.css';
</style>
