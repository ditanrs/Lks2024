<script setup>
definePageMeta({
  middleware: "auth",
});
const user = useSupabaseUser();
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
          <td>email</td>
          <td>aktivitas</td>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td value="#"></td>
          <td></td>
          <td></td>
          <td></td>
          <td></td>
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
