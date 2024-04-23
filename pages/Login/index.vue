<script setup>
definePageMeta({
  layout: "login",
});
const supabase = useSupabaseClient();
const email = ref("");
const password = ref("");

async function handleLogin() {
  const { error } = await supabase.auth.signInWithPassword({
    email: email.value,
    password: password.value,
  })
  if (error) throw error
  else {
    const { data } = await supabase.from("users").select("id").eq("email", email.value);
    if (data) {
      console.log(data)
      const { error } = await supabase.from("Log_Activity").insert({
        aktifitas: "Login",
        id_user: data[0].id,
      });
      if (error) throw error
      else navigateTo('/')
    }
  }
}
</script>

<template>
  <div class="logo1">
    <div class="container-fluid">
      <div>
        <img src="assets/img/logo.png" alt="logo" class="logo" />
        <h1>APOTEX XYZ</h1>
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
  </div>
</template>

<style scoped>
.container-fluid {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 35%;
}
.logo1 {
  background-color: #87bc9c;
}
.form-control {
  margin-bottom: 6px;
  width: 100%;
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
  background-color: #019901 !important;
}
</style>
