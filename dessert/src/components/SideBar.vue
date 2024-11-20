<template>
  <nav>
    <v-navigation-drawer dark app color="#FFCB5E" width="100">
      <div class="text-center mt-5">
        <v-icon color="#4D2C00" large class="mt-4">fas fa-bars</v-icon>
      </div>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {
  name: "SideBar",
  data: () => ({
    selectedItem: 0,
    drawer: null,
    items: [
      { icon: "fas fa-apple-alt", text: "Discover" },
      { icon: "fas fa-carrot", text: "Stream" },
      { icon: "fas fa-leaf", text: "Community" },
      { icon: "fas fa-lemon", text: "Statistics" },
      { icon: "fas fa-pepper-hot", text: "Statistics" },
      { icon: "fas fa-seedling", text: "Statistics" },
    ],
  }),
};
</script>

<style></style>
