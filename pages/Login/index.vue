<script setup>
definePageMeta({
  layout: "login",
});
const supa = useSupabaseClient();
const email = ref("");
const password = ref("");

async function handleLogin() {
  const { data, error } = await supa.auth.signInWithPassword({
    email: email.value,
    password: password.value,
  });
  if (!error) navigateTo("/");
}
</script>

<template>
  <div class="container-fluid">
    <div class="logo1">
      <div>
        <img src="assets/img/logo.png" alt="logo" class="logo" />
        <h1>APOTEX XYZ</h1>
      </div>
    </div>
    <form @submit.prevent="handleLogin">
      <div class="mb-3">
        <input v-model="email" type="email" class="form-control form-control-lg rounded-2 border-dark" placeholder="email" />
      </div>
      <br />
      <input v-model="password" type="password" class="form-control form-control-lg rounded-2 border-dark" placeholder="password" />
      <br />
      <button type="submit" class="btn btn-success text-white rounded-2 px-4 text-center">LOGIN</button>
    </form>
  </div>
</template>

<style scoped>
.container-fluid {
  background-color: #87bc9c;
  width: 100vw;
  
}
.logo1 {
  display: flex;
  justify-content: center;
  margin-top: 120px;
}
.form-control {
  margin-bottom: 6px;
  width: 30%;
  margin-left: 35%;
}
h1 {
  margin-top: 15px;
  margin-bottom: 20px;
}
.logo {
  width: 95px;
  margin-left: 30%;
}
.btn {
  margin-left: 47%;
  background-color: #019901 !important;
}
</style>
