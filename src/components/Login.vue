<template>
  <!-- Material form login -->
  <form>
    
    <p class="h4 text-center mb-10">Sign in</p>
    <div class="h4 text-center mb-4">
      <mdb-input icon="envelope" type="email" placeholder="  Email"/>
      <mdb-input icon="lock" type="password"  placeholder="  Password"/>
    </div>
    <div class="text-center">
      <mdb-btn>Connect</mdb-btn>
      
    </div>

    <div class="text-center">
      <mdb-btn>Sign Up</mdb-btn>
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