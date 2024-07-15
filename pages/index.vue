<script setup>
definePageMeta({
  middleware: "auth",
});
const counter = useCounter();
</script>

<template>
  <div>
    <div>
      Counter :{{ counter }}
      <button @cliick="counter++">+</button>
      <button @cliick="counter--">-</button>
    </div>

    <ContentDoc />
    <ProfileHeader />
    <Alert />
    <Profile />
  </div>
</template>
