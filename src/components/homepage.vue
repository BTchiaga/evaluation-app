<template>
  <v-container>
    <v-row class="text-center justify-center">
      <v-col cols="12"> </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Welcome to this evaluation app
        </h1>

        <p class="subheading font-weight-regular">Study Description</p>
      </v-col>

      <v-col class="mb-5" cols="12">
        <v-row justify="center">
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Velit
            quibusdam, optio, repellat distinctio id quisquam itaque aperiam
            minus magni nemo, amet cum! Modi pariatur tempore temporibus
            consequatur alias placeat odio?
          </p>
        </v-row>
      </v-col>

      <v-col class="mb-5" cols="12">
        <v-row justify="center">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda,
            laudantium quidem? Autem nulla recusandae fugit laboriosam similique
            tempore, iusto vel, commodi sequi minus aliquam consequuntur
            necessitatibus, placeat quod nihil nesciunt.
          </p>
        </v-row>
      </v-col>

      <v-col class="mb-6" cols="12">
        <v-row justify="center">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste,
            repellendus omnis. Minima suscipit a harum distinctio aliquid
            placeat, provident quos tempora, ullam earum voluptas, officiis
            illum maxime culpa. Doloremque, aperiam.
          </p>
        </v-row>
      </v-col>
    </v-row>
    <div class="d-flex justify-center my-6">
      <v-btn elevation="2" outlined @click="gotoAboutYou">Go</v-btn>
    </div>
  </v-container>
</template>

<script>
export default {
  name: "homepage",

  data: () => ({}),

  methods: {
    gotoAboutYou() {
      this.$router.push("about");
    },
  },
};
</script>
