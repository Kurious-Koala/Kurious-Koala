<template>
  <div class="home">
    <img class="logo" alt="logo" src="../assets/logo.jpeg" />
    <HomePage msg="Welcome to our Online Game" />
  </div>
</template>

<script>
// @ is an alias to /src
import HomePage from "@/components/HomePage.vue";

export default {
  name: "Home", 
  components: {
    HomePage,
  },
};
</script>

<style scoped>
.logo {
  border-radius: 50%;
}
</style>
