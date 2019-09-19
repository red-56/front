<template>
  <!-- Material form login -->
  <form>
    
    <p class="h4 text-center mb-10">Sign in</p>
    <div class="h4 text-center mb-4">
      <mdb-input icon="envelope" type="email" placeholder="  Email"/>
      <mdb-input icon="lock" type="password"  placeholder="  Password"/>
    </div>
    <div class="text-center">
      <router-link to="/">
      <mdb-btn>Connect</mdb-btn>
      </router-link>
      
    </div>

    <div class="text-center">
      <router-link to="/signup">
      <mdb-btn>Sign Up</mdb-btn>
      </router-link>
    </div>
   
  </form>
  <!-- Material form login -->
</template>

<script>
  import { mdbInput, mdbBtn } from 'mdbvue';
  export default {
    name: 'Basic',
    components: {
      mdbInput,
      mdbBtn
    },
  }
</script>