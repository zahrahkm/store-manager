<template>
  <div class="login">
    <div class="container">
      <img src="../assets/images/online-store.png" alt="online-store" />
      <div class="seperator"></div>
      <form>
        <h1>Sign in</h1>
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
}
form {
  width: 100%;
  display: flex;
  flex-direction: column;
  margin-top: 1rem;
}
form h1 {
  text-align: center;
  margin-bottom: 10px;
  color: #c2410c;
  font-weight: 800;
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
  cursor: pointer;
  transition-duration: 0.1s;
}
form button:hover {
  background-color: #fed7aa;
}

@media (min-width: 640px) {
  .login {
    padding: 4rem 8rem;
  }
}

@media (min-width: 1024px) {
  .login {
    display: flex;
    align-items: center;
  }
  .container {
    flex-direction: row;
  }
  .container img {
    width: 42%;
  }
  form {
    margin-top: 0;
  }
  form h1 {
    text-align: left;
  }
  .seperator {
    height: 5rem;
    width: 1px;
    margin: 0 2rem;
  }
}
@media (min-width: 1280px) {
  .login {
    padding: 4rem 16rem;
  }
}
</style>
