<template>
  <div class="koala">
    <img class="koala" alt="koala" src="./assets/KoalaNavbar.png" />
  </div>
  <div id="nav">
    <router-link to="/" :style="{ color: black }">Home</router-link>
    <router-link to="/about" :style="{ color: black }">About</router-link>
    <router-link to="/levels" :style="{ color: black }">Levels</router-link>
    <router-link to="/login" :style="{ color: black }">Login</router-link>
    <select class="languageSelector" v-model="currentLocale">
      <option
        class="optionLanguage"
        v-for="locale in locales"
        :value="locale.value"
        :key="locale.value"
      >
        {{ locale.id }}
      </option>
    </select>
  </div>
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
  color: "black";
  font-size: 24px;
}

.koala {
  width: 60px;
  height: 60px;
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

.languageSelector {
  border: none;
  font-weight: bold;
}

.optionLanguage {
  border: none;
  color: "black";
  font-size: 24px;
}

/***************   RESPONSIVE DESIGN   ***************/

/*** mobile phones view ***/
@media (min-width: 575px) {

}

/*** tablets view ***/
@media (min-width: 768px) {
 
}

/*** desktop view ***/
@media (min-width: 992px) {

}

/*** extra large desktop view ***/
@media (min-width: 1200px) {

}
</style>
