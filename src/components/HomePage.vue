<template>
  <div class="HomePage" v-if="appear">
    <img class="HomePage__logo" alt="logo" src="../assets/logo.jpg" />
    <h1 class="HomePage__header" :style="{ color: green }">{{ msg }}</h1>
    <button class="HomePage__playBtn" @click="start" :disabled="isPlaying">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="45"
        height="45"
        fill="currentColor"
        class="bi bi-play-circle-fill"
        viewBox="0 0 16 16"
      >
        <path
          d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM6.79 5.093A.5.5 0 0 0 6 5.5v5a.5.5 0 0 0 .79.407l3.5-2.5a.5.5 0 0 0 0-.814l-3.5-2.5z"
        />
      </svg>
    </button>
  </div>
  <GameLevel1 v-if="isPlaying" />
</template>

<script>
import GameLevel1 from "../components/GameLevel1.vue";

export default {
  name: "HomePage",
  props: {
    msg: String,
  },
  components: { GameLevel1 },
  data() {
    return {
      isPlaying: false,
      delay: null,
      appear: true,
      green: "#087d12",
    };
  },
  methods: {
    start() {
      this.delay = 2000 + Math.random() * 5000;
      this.isPlaying = true;
      console.log(this.delay);
      this.appear = false;
    },
  },
};
</script>

<style scoped>
.HomePage__logo {
  width: 250px;
  height: 320px;
}

.HomePage__header {
  margin-top: 20px;
  font-family: Ribeye;
  font-size: 30px;
}

.HomePage__playBtn {
  margin: 40px 0 50px;
  background-color: Transparent;
  background-repeat: no-repeat;
  border: none;
  cursor: pointer;
  overflow: hidden;
}
</style>
