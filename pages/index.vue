<script setup>
definePageMeta({
  middleware: "auth",
});
</script>

<template>
  <div>
    <ContentDoc />
    <ProfileHeader />
    <Alert />
    <Profile />
  </div>
</template>
