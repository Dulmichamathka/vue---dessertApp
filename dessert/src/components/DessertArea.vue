<template>
  <v-item-group mandatory class="mt-n4">
    <v-container>
      <v-row justify="center" class="space">
        <v-col
          cols="12"
          xs="12"
          md="2"
          v-for="(category, i) in categories"
          :key="i"
        >
          <v-item v-slot="{ active, toggle }">
            <v-card
              :color="active ? '#FFCB5E' : 'white'"
              :class="active ? 'borderme' : 'borderout'"
              class="d-flex align-center rounded-lg mx-2"
              dark
              height="120"
              @click="toggle"
              flat
            >
              <v-row>
                <v-col cols="12" sm="12">
                  <v-list-item three-line class="text-center">
                    <v-list-item-content>
                      <div align="center" justify="center">
                        <v-img
                          :src="category.img"
                          max-height="100"
                          max-width="120"
                          style="border-radius: 10px; object-fit: cover"
                          contain
                        ></v-img>
                      </div>
                    </v-list-item-content>
                  </v-list-item>
                </v-col>
              </v-row>
            </v-card>
          </v-item>
        </v-col>
      </v-row>
    </v-container>
  </v-item-group>
</template>

<script>
export default {
  data: () => ({
    categories: [
      {
        img: "1.png",
      },
      {
        img: "2.png",
      },
      {
        img: "3.png",
      },
      {
        img: "4.png",
      },
      {
        img: "5.png",
      },
    ],
  }),
};
</script>
<style></style>
