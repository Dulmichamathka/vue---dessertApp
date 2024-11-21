<template>
  <v-row class="mt-n2">
    <v-col cols="12" sm="1">
      <v-avatar size="60" class="ml-4 mt-4 bordered">
        <v-img src="img6.jpg"></v-img>
      </v-avatar>
    </v-col>

    <v-col cols="12" sm="11">
      <v-rating
        v-model="rating"
        background-color="grey "
        color="grey"
        x-small
      ></v-rating>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui molestias
        veniam illo tempora officia distinctio ipsa quisquam sint alias
        temporibus. Vel, maxime. Itaque corporis possimus unde vitae ipsam
        blanditiis mollitia!
      </p>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    rating: 4,
  }),
};
</script>
<style></style>
