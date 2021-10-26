<template>
  <div v-if="ShowDescription">
    <Description />
  </div>
</template>

<script>
import Description from "../components/Description.vue";
export default {
  name: "About",
  components: {
    Description,
  },
  data() {
    return {
      text: "become a member and take -10%",
      ShowDescription: true,
    };
  },
  methods: {
    handleDescription() {
      this.ShowDescription = !this.ShowDescription;
    },
  },
};
</script>
