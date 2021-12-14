<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import ProfileCard from "./components/ProfileCard.vue";
import ProfileCardSkeleton from "./components/ProfileCardSkeleton.vue";
</script>

<template>
  <Suspense>
    <template #default>
      <ProfileCard />
    </template>
    <template #fallback>
      <ProfileCardSkeleton />
    </template>
  </Suspense>
</template>

<style>
html,
body {
  background-color: #eee;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
