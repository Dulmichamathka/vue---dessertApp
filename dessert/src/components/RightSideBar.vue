<template>
  <v-navigation-drawer app color="#fff" right width="290">
    <v-toolbar color="transparent" flat>
      <h4>Today's menu</h4>
      <v-spacer></v-spacer>
      <v-badge bordered bottom color="red" dot offset-x="8" offset-y="30">
        <v-avatar size="30">
          <v-img src="../assets/profile.jpg"></v-img>
        </v-avatar>
      </v-badge>
    </v-toolbar>

    <v-card
      class="d-flex align-center rounded-lg mx-2 borderme"
      color="white"
      flat
      dark
      @click="toggle"
    >
      <v-row>
        <v-col cols="12" sm="12">
          <v-list-item three-line class="text-center">
            <v-list-item-content>
              <div align="center" justify="center">
                <v-img
                  src="../assets/1.jpeg"
                  max-height="280"
                  max-width="200"
                ></v-img>
              </div>
              <v-toolbar flat color="transparent" class="mt-n4">
                <v-rating
                  v-model="rating"
                  background-color="orange lighten-3"
                  color="orange"
                  x-small
                ></v-rating>

                <v-spacer></v-spacer>
                <h6 class="black--text">$13</h6>
              </v-toolbar>
            </v-list-item-content>
          </v-list-item>
        </v-col>
      </v-row>
    </v-card>

    <h4 class="black--text ml-4 mt-6 mb-4">Person</h4>
    <v-row>
      <v-col cols="12" sm="8">
        <v-slider
          v-model="ex3.val"
          :thumb-color="ex3.color"
          thumb-label="always"
          class="mt-10"
        ></v-slider>
      </v-col>

      <v-col cols="12" sm="4" class="pl-0">
        <v-img src="../assets/shopping-bags.gif"></v-img>
      </v-col>
    </v-row>
    <h4 class="ml-5 mt-n6">Summery</h4>
    <v-row class="mt-5">
      <v-col cols="12" sm="3">
        <v-card class="rounded-xl ml-2" flat>
          <v-img
            src="../assets/chocolate.jpg"
            max-height="100%"
            max-width="100%"
            contain
          ></v-img>
        </v-card>
      </v-col>
      <v-col cols="12" sm="7">
        <h4 class="mt-1">1X Best chocolate</h4>
      </v-col>
      <v-col cols="12" sm="2">
        <h6 class="mt-2 grey--text">$13</h6>
      </v-col>
      <v-col cols="12" sm="3">
        <v-card
          class="rounded-xl ml-2 borderme d-flex align-center py-1"
          flat
          color="white"
        >
          <v-icon class="ml-3" small>fas fa-truck</v-icon>
        </v-card>
      </v-col>
      <v-col cols="12" sm="7">
        <h4 class="mt-1">Delivery</h4>
      </v-col>
      <v-col cols="12" sm="2">
        <h6 class="mt-2 grey--text">$00</h6>
      </v-col>
      <v-col cols="12" sm="3"></v-col>
      <v-col cols="12" sm="7">
        <h4 class="mt-1">Total</h4>
      </v-col>
      <v-col cols="12" sm="2">
        <h6 class="mt-2 grey--text ml-n4">$13.99</h6>
      </v-col>
    </v-row>
    <v-toolbar class="mt-2" flat color="transparent">
      <h4 color="black--text">Person <strong>20</strong></h4>
      <v-spacer></v-spacer>
      <v-btn color="#ffcb5e">
        Checkout
        <v-icon color="black" right>fas fa-arrow-right</v-icon>
      </v-btn>
    </v-toolbar>
  </v-navigation-drawer>
</template>

<script>
export default {
  data: () => ({
    rating: 4,
    ex3: {
      val: 20,
      color: "red",
    },
  }),
};
</script>

<style>
.v-card.borderme {
  border: 2px solid #4d2c00 !important;
}
.v-card.borderout {
  border: 1px solid #d5f0db !important;
}
</style>
