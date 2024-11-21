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
                          max-height="60"
                          max-width="80"
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
        img: "https://cdn.loveandlemons.com/wp-content/uploads/2021/06/summer-desserts.jpg",
      },
      {
        img: "https://www.allrecipes.com/thmb/rOSWRQmSwBjWyAnnCVJcpd5xBnM=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/3574694-hot-fudge-ice-cream-bar-dessert-Allrecipes-Magazine-4x3-1-8b0b0580bfb14ae9bb8a9b3acb421ad5.jpg",
      },
      {
        img: "https://cdn.apartmenttherapy.info/image/upload/v1709316229/k/Edit/2024-03-cherry-delight/cherry-delight2.jpg",
      },
      {
        img: "https://img.freepik.com/premium-photo/decadent-chocolate-lava-cake-with-molten-center-perfect-dessert-combines-rich-chocolate_817921-4530.jpg",
      },
      {
        img: "https://dancearoundthekitchen.com/wp-content/uploads/2022/08/DSC_1822.jpg",
      },
    ],
  }),
};
</script>
<style></style>
