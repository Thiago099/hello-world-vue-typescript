<template>
  <div class="container">
    <div>
      <div class="row">
        <div class="form-group">
          <label for="exampleInputEmail1">Email address</label>
          <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email">
          <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
        </div>
        <div class="form-group">
          <label for="exampleInputPassword1">Password</label>
          <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
        </div>
        <div class="form-group">
          <input type="checkbox" class="form-check-input" id="exampleCheck1">
          <label class="form-check-label" for="exampleCheck1">Stay logged in</label>
        </div>
        <div class="form-group">
          <button type="submit" style="float:right" class="btn btn-primary">Log in</button>
        </div>
      </div>

    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'HomePage',
});
</script>
<style scoped>
.form-group{
  margin-bottom: 1rem;
}
input[type="checkbox"]{
  margin-right: .5rem;
}
.container{
  max-width: 500px;
}
</style>
