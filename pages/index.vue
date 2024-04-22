<template>
  <div class="mt-5 text-center">
    {{ user }}
  </div>
</template>
<script setup>
definePageMeta({
  middleware: "auth",
});
const user = useSupabaseUser();
</script>
