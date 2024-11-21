<template>
  <v-app :style="{ background: $vuetify.theme.themes.dark.background }">
    <SideBar />
    <RightSideBar />
    <v-container>
      <NavBar />
      <DessertArea />
      <v-toolbar class="mt-n4" flat color="transparent">
        <v-toolbar-title class="ml-4">
          <strong>Day</strong> <span class="grey--text ml-2">Menu</span>
        </v-toolbar-title>
      </v-toolbar>
      <MenuArea />
      <v-toolbar class="mt-n4" flat color="transparent">
        <v-toolbar-title class="ml-4">
          <strong>Ingredients</strong> <span class="grey--text ml-2">Food</span>
        </v-toolbar-title>
      </v-toolbar>
      <FoodCom />
      <Comment />
    </v-container>
  </v-app>
</template>

<script>
import SideBar from "../components/SideBar";
import RightSideBar from "../components/RightSideBar.vue";
import NavBar from "../components/NavBar";
import DessertArea from "../components/DessertArea";
import MenuArea from "../components/MenuArea";
import FoodCom from "../components/FoodCom";

export default {
  name: "HomeView",

  components: {
    SideBar,
    RightSideBar,
    NavBar,
    DessertArea,
    MenuArea,
    FoodCom,
  },
};
</script>
