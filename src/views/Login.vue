<template>
  <div class="login">
    <div class="container">
      <img src="../assets/images/online-store.png" alt="online-store" />
      <div class="seperator"></div>
      <h1>Sign in</h1>
      <form>
        <div class="form-control">
          <label>Username</label>
          <input type="text" name="username" />
        </div>
        <div class="form-control">
          <label>Password</label>
          <input type="password" name="password" />
        </div>
        <button type="submit">Login</button>
      </form>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Login",
  components: {}
});
</script>

<style scoped>
.login {
  background-color: #fdba74;
  min-height: 100vh;
  padding: 1rem;
}
.container {
  background-color: white;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.25);
  width: 100%;
  padding: 2rem;
  margin: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.container img {
  width: 75%;
}
.seperator {
  height: 1px;
  width: 25%;
  background-color: rgba(124, 44, 18, 0.3);
  margin-bottom: 15px;
}
form {
  width: 100%;
  display: flex;
  flex-direction: column;
  margin-top: 15px;
}
.form-control {
  font-size: 14px;
  margin-top: 10px;
  display: flex;
  flex-direction: column;
}
.form-control label {
  font-weight: bold;
}
.form-control input {
  font-size: 14px;
  border: none;
  border-bottom: 1px solid #7c2d12;
  padding: 8px;
  margin: 5px 0;
}
.form-control input:focus {
  outline: none;
  border: 1px solid #7c2d12;
}
form button {
  font-size: 14px;
  font-weight: bold;
  border: none;
  background-color: #fdba74;
  padding: 12px;
  margin-top: 30px;
}
</style>
