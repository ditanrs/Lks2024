<script setup>
const supabase = useSupabaseClient();

async function logout() {
  const { error } = await supabase.auth.signOut();
  if (!error) navigateTo("/Login");
}
onMounted(() => {
  logout();
});
</script>

<template>
  <h3 class="text-center">Loading...</h3>
  <h3 class="text-center">Anda sedang keluar dari aplikasi ini</h3>
</template>
