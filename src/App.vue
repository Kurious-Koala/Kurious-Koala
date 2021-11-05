<template>
  <div class="koala">
    <img class="koala" alt="koala" src="./assets/KoalaNavbar.png" />
  </div>
  <div id="nav">
    <router-link to="/" :style="{ color: black }">Home</router-link>
    <router-link to="/about" :style="{ color: black }">About</router-link>
    <router-link to="/levels" :style="{ color: black }">Levels</router-link>
    <router-link to="/login" :style="{ color: black }">Login</router-link>
    <select v-model="currentLocale">
      <option v-for="locale in locales" v-bind:key="locale.id">
        {{ locale.name }}
      </option>
    </select>
  </div>
  <!-- <img class="globe" alt="globe" src="./assets/globe.svg" /> -->
  <router-view />
  <Footer />
</template>

<script>
// @ is an alias to /src
import Footer from "@/components/Footer.vue";
export default {
  name: "App",
  components: {
    Footer,
  },
  el: "#app",
  data() {
    return {
      green: "#087d12",
      black: "#000000",
      lightGreen: "#96d19b",
      locales: [
        { id: "en", name: "English" },
        { id: "gr", name: "Greek" },
        { id: "sv", name: "Swedish" },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: "Henny Penny", cursive;
  text-align: center;
  color: 'black';
  font-size: 24px;
}

.koala {
  width: 80px;
  height: 80px;
  margin: auto 240px;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: "black";
  padding: 0 20px;
}

</style>
