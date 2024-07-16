<script setup>
const response = await $fetch("/api/hello");
console.log(response);

definePageMeta({
  middleware: "auth",
});
import { useCounterStore } from "~/stores/myStore";
// const counter = useCounter();
const { count, increment, decrement } = useCounterStore();
</script>

<template>
  <div>
    <div>
      {{ count }}
      <button @click="increment">+</button>
      <button @click="decrement">-</button>
    </div>

    <ContentDoc />
    <ProfileHeader />
    <Alert />
    <Profile />
  </div>
</template>
