<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <v-btn class="mx-2" fab dark small color="primary">
        <v-icon dark> mdi-plus </v-icon>
      </v-btn></v-app-bar
    >
    <v-main>
      <div class="peer-main">
        <UserIcon />
      </div>
    </v-main>

    <div>
      <HomeFooter />
    </div>
  </v-app>
</template>
 
<script>
import UserIcon from "./components/UserIcon";
import HomeFooter from "./components/HomeFooter.vue";

export default {
  name: "App",

  components: {
    HomeFooter,
    UserIcon,
  },

  methods: {},

  data: () => ({
    //
  }),
};
</script>

<style scoped>
.peer-main {
  width: 100%;
  overflow: hidden;
  flex-flow: row wrap;
  z-index: 2;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
