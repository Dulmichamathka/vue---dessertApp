<template>
  <v-app :style="{ background: $vuetify.theme.themes.dark.background }">
    <SideBar />
    <RightSideBar />
    <v-container>
      <NavBar />
      <DessertArea />
    </v-container>
  </v-app>
</template>

<script>
import SideBar from "../components/SideBar";
import RightSideBar from "../components/RightSideBar.vue";
import NavBar from "../components/NavBar";
import DessertArea from "../components/DessertArea";

export default {
  name: "HomeView",

  components: {
    SideBar,
    RightSideBar,
    NavBar,
    DessertArea,
  },
};
</script>
