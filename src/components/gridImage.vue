<template>
  <v-card class="mx-auto px-4">
    <v-card-text>
      <div>clustered images</div>
    </v-card-text>
    <v-row class="margin-image">
      <v-col v-for="n in 9" :key="n" class="d-flex child-flex" cols="3">
        <v-img
          :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
          :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
          aspect-ratio="2"
          class="grey lighten-2 px-2"
        >
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular
                indeterminate
                color="grey lighten-5"
              ></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>
  </v-card>
</template>
<script>
export default {
  name: "gridImage",

  data() {
    return {};
  },
};
</script>

<style scoped>
.v-sheet.v-card {
  border-radius: -32px;
  width: 69em;
  margin: auto;
}
.row.margin-image {
  margin: auto;
}
</style>
