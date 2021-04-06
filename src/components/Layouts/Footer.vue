<template>
  <v-footer app absolute color="#141618" dark>
    <v-container class="py-16">
      <v-row justify="space-around" align="start">
        <v-col cols="12" md="4" lg="3">
          <div class="body-1">
            Subscribe to the Email Newsletter
          </div>

          <div class="d-flex mt-2">
            <v-text-field
              solo
              outlined
              flat
              hide-details
              label="Your email address"
              class="rounded-r-0 "
            />
            <v-btn height="56" light class="text-capitalize rounded-l-0"
              >Subscribe</v-btn
            >
          </div>
        </v-col>

        <v-col cols="12" md="4" lg="3">
          <div class="body-1">
            Follow Author on
          </div>

          <div class="mt-2">
            <v-row>
              <v-col cols="4">
                <v-btn large block
                  ><v-icon left>mdi-twitter</v-icon> Twitter</v-btn
                >
              </v-col>

              <v-col cols="4">
                <v-btn large block
                  ><v-icon left>mdi-github</v-icon> Github</v-btn
                >
              </v-col>

              <v-col cols="4">
                <v-btn large block
                  ><v-icon left>mdi-feather</v-icon> HeroUI</v-btn
                >
              </v-col>
            </v-row>
          </div>
        </v-col>

        <v-col cols="12" md="4" lg="3">
          <div class="body-1">
            ©2021 HeroUI
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-footer>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<style scoped></style>
