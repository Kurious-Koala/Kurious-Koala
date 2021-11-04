<template>
  <div class="koala">
    <img class="koala" alt="koala" src="./assets/KoalaNavbar.png" />
  </div>
  <div id="nav">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
    <router-link to="/levels">Levels</router-link>
    <router-link to="/login">Login</router-link>
    <select v-model="currentLocale">
      <option v-for="locale in locales" v-bind:key="locale.id">
        {{ locale.name }}
      </option>
    </select>
    <p class="welcome-msg">{{ message[currentLocale] }}</p>
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
      message: {
        en: "Welcome to kurious Koala",
        gr: "Καλώς ήρθατε στο kurious Koala",
        sv: "Välkomna till kurious Koala",
      },
      currentLocale: "en",
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
  color: #000000;
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
  color: #000000;
  padding: 0 20px;
}

.koala:hover {
  color: #96d19b;
}

#nav a.router-link-exact-active {
  color: #96d19b;
}

.welcome-msg {
  font-family: "Ribeye Marrow";
  color: #087d12;
  font-size: 30px;
  padding-top: 50px;
}
</style>
