<template>
  <!-- Material form register -->
  <form>
    <p class="h4 text-center mb-4">Sign up</p>
    <div class="h4 text-center mb-4">
      <mdb-input icon="user" type="text" placeholder="  Your name"/>
      <mdb-input  icon="envelope" type="email" placeholder="  Your email"/>
      <mdb-input  icon="exclamation-triangle" type="text" placeholder="  Confirm your email"/>
      <mdb-input  icon="lock" type="password" placeholder="  Your password"/>
    </div>
    <div class="text-center">
         <router-link to="/">
      <mdb-btn color="primary">Register</mdb-btn>
      </router-link>
    </div>
  </form>
  <!-- Material form register -->
</template>

<script>
  import { mdbInput, mdbBtn } from 'mdbvue';
  export default {
    name: 'Basic',
    components: {
    mdbInput,
    mdbBtn
    }
};
</script>
