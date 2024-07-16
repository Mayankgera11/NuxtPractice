<script setup>
definePageMeta({
  middleware: "auth",
});
import { useCounterStore } from "~/stores/myStore";
// const counter = useCounter();
const store = useCounterStore();
</script>

<template>
  <div>
    <div>
      {{ store.count }}
      <button @click="store.increment">+</button>
      <button @click="store.decrement">-</button>
    </div>

    <ContentDoc />
    <ProfileHeader />
    <Alert />
    <Profile />
  </div>
</template>
