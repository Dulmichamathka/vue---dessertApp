<template>
  <v-app :style="{ background: $vuetify.theme.themes.dark.background }">
    <SideBar />
    <v-container> </v-container>
  </v-app>
</template>

<script>
import SideBar from "../components/SideBar";

export default {
  name: "HomeView",

  components: {
    SideBar,
  },
};
</script>
