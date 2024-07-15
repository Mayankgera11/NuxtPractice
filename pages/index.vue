<script setup>
const { sayHello } = UseUtils();
sayHello();
</script>

<template>
  <div>
    <ProfileHeader />
    <Alert />
    <Profile />
  </div>
</template>
