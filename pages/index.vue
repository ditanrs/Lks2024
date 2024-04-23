<script setup>
definePageMeta({
  middleware: "auth",
});
const supabase = useSupabaseClient();
const user = useSupabaseUser();

const logs = ref([]);
async function getLog() {
  const { data, error } = await supabase.from("Log_Activity").select(`
    *,
    users (username)
  `);
  if (error) throw error;
  if (data) logs.value = data;
}

onMounted(() => {
  getLog();
});
</script>
<template>
  <div class="container-fluid">
    <div class="text-center mt-5">
      <h3>Log Activity</h3>
    </div>
    <table class="table">
      <thead class="table-dark">
        <tr>
          <td>No</td>
          <td>username</td>
          <td>Waktu</td>
          <td>aktivitas</td>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(log, index) in logs">
          <td value="#">{{ index + 1 }}</td>
          <td>{{ log.users.username }}</td>
          <td>{{ log.waktu }}</td>
          <td>{{ log.aktifitas }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<style scoped>
table {
  width: 70%;
  margin-left: 15%;
  margin-top: 5%;
}
</style>
