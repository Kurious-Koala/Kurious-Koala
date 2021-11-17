<template>
  <div class="KuriousKoala">
    <img
      class="KuriousKoala__img"
      alt="KuriousKoalaImg"
      src="./assets/KoalaNavbar.png"
    />
  </div>
  <div id="nav">
    <router-link to="/" :style="{ color: lightGreen }">Home</router-link>
    <router-link to="/about" :style="{ color: lightGreen }">About</router-link>
    <router-link to="/levels" :style="{ color: lightGreen }"
      >Levels</router-link
    >
    <router-link to="/login" :style="{ color: lightGreen }">Login</router-link>
    <select class="nav__languageSelector" v-model="currentLocale">
      <option
        class="nav__languageSelector--option"
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
  font-size: 10px;
}

.KuriousKoala__img {
  width: 30px;
  height: 30px;
}

#nav {
  padding: 30px;
}

#nav a {
  padding: 0 20px;
}

#nav a:hover {
  padding: 0 20px;
  text-decoration-line: none;
  text-shadow: 1px 1px;
}

.nav__languageSelector {
  border: none;
  background-color: transparent;
}

.nav__languageSelector--option {
  border: none;
  font-size: 24px;
}

/***************   RESPONSIVE DESIGN   ***************/

/*** Extra small devices only ***/
@media (max-width: 767px) {
  .KuriousKoala__img {
    width: 40px;
    height: 40px;
  }
  #app {
    font-size: 14px;
  }
}

/*** Small devices only ***/
@media (min-width: 768px) and (max-width: 991px) {
  .KuriousKoala__img {
    width: 60px;
    height: 60px;
    justify-content: flex-end;
  }
  #app {
    font-size: 18px;
  }
}

/*** Medium devices only ***/
@media (min-width: 992px) and (max-width: 1199px) {
  .KuriousKoala__img {
    width: 70px;
    height: 70px;
  }
  #app {
    font-size: 24px;
  }
}

/*** extra large desktop view ***/
@media (min-width: 1200px) {
  .KuriousKoala__img {
    width: 80px;
    height: 80px;
  }
  #app {
    font-size: 26px;
  }
}
</style>
