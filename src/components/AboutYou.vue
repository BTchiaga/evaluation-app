<template>
  <v-container class="aboutYouContainer">
    <v-row class="text-center justify-center">
      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">About You</h1>
        <div>
          <p>Age: {{ age }}</p>
          <v-col cols="12" sm="6" md="3">
            <v-text-field
              v-model="age"
              label="Age"
              placeholder="Enter your age"
              outlined
              :rules="rules"
              type="number"
            ></v-text-field>
          </v-col>
        </div>
      </v-col>
    </v-row>
    <v-row class="mt-12">
      <v-col cols="12" sm="4" md="4">
        <span>Glasses:</span>
        <p>{{ glasses }}</p>

        <v-checkbox
          v-model="glasses"
          label="yes"
          color="secondary"
          value="yes"
          hide-details
        ></v-checkbox>
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
export default {
  name: "AboutYou",
  glasses: String,
  age: Number,

  data() {
    return {
      glasses: "",
      age: 0,
      min: 18,
      max: 90,
      rules: [(v) => v >= 99 || "Min Age 18 and Max age 99"],
    };
  },
};
</script>
