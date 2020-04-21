<template>
  <div class="auth-page">
    <div class="first">
      <h1>Log in to advertisement, so you can post your ads</h1>
      <p>Enter your details to login</p>
    </div>
    <div class="auth-container">
      <form>
        <AppControlInput type="email">E-mail address</AppControlInput>
        <AppControlInput type="password">Password</AppControlInput>
        <AppButton type="submit">{{ isLogin ? 'Login' : 'Sign Up' }}</AppButton>
        <AppButton
          type="button"
          btn-style="inverted"
          style="margin-left: 10px"
          @click="isLogin = !isLogin"
        >Switch to {{ isLogin ? 'Signup' : 'Login' }}</AppButton>
      </form>
    </div>
  </div>
</template>

<script>
import AppControlInput from "@/components/UI/AppControlInput";
import AppButton from "@/components/UI/AppButton";

export default {
  name: "AdminAuthPage",
  components: {
    AppControlInput,
    AppButton
  },
  data() {
    return {
      isLogin: true
    };
  },
  head: {
    title: "Login"
  }
};
</script>

<style scoped>
.auth-page {
  padding: 80px;
  height: 100vh;
  display: flex;
  align-items: center;
  background-image: url("~assets/images/bc.jpg");
}

.first {
  width: 50%;
}

.first h1 {
  font-size: 30px;
  color: #073b5e;
}

.first p {
  font-size: 22px;
  color: #747391;
}
.auth-container {
  border: 2px solid #505253;
  border-radius: 5px;
  box-shadow: 0 5px 5px #8c9092;
  margin: auto;
  padding: 10px;
  box-sizing: border-box;
  text-align: center;
  justify-content: center;
  width: 50%;
  padding: 0px 20px 20px 20px;
}
</style>

