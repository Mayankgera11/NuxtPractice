<script setup>
const { $sayHello } = useNuxtApp();
$sayHello("mayank");
</script>

<template>
  <div>
    <ProfileHeader />
    <Alert />
    <Profile />
  </div>
</template>
