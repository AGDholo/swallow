<template>
  <v-row justify="space-around" align="center">
    <v-col
      cols="12"
      md="6"
      lg="5"
      :order="$vuetify.breakpoint.smAndDown ? 10 : 1"
    >
      <v-card color="transparent" flat>
        <div class="d-flex align-center">
          <v-chip color="indigo" small class="subtitle-2"> Tutorials</v-chip>
          <div class="ml-2 body-2 grey--text text--lighten-1">
            February 3rd, 2021
          </div>
        </div>

        <div class="text-h3 my-5">
          Ut enim blandit volutpat maecenas
        </div>

        <div class="text-h6 font-weight-regular">
          Duis aute irure dolor in reprehenderit in voluptate velit esse cillum
          dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
          proident, sunt in culpa qui officia deserunt mollit anim id est
          laborum.
        </div>
      </v-card>
    </v-col>

    <v-col cols="12" md="6" lg="5" order="2">
      <v-card color="transparent" flat>
        <v-img
          class="rounded-lg"
          src="https://cdn.pixabay.com/photo/2021/02/04/12/47/boat-5981235_1280.jpg"
        ></v-img>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style scoped></style>
