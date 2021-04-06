<template>
  <div>
    <v-sheet color="#141618" dark class="py-16">
      <v-container class="pt-2 my-16">
        <Header />

        <v-row justify="space-around" align="center" class="my-16 py-16">
          <v-col cols="12" md="4" lg="3" v-for="item in 3" :key="item">
            <simple-card
              image="https://cdn.pixabay.com/photo/2021/01/30/18/07/salzburg-5964812_1280.jpg"
              category="News"
              date="February 3rd, 2021"
              title="Ut enim blandit volutpat maecenas volutpat blandit"
              category-color="deep-purple"
              flat
              color="transparent"
            />
          </v-col>
        </v-row>

        <v-row justify="space-around" align="center" class="mt-16">
          <v-col cols="12" md="6" lg="5">
            <InfoCard
              title="Newsletter"
              subtitle="Duis aute irure dolor in reprehenderit in voluptate velit
                      esse cillum dolore."
              light
              class="pa-10"
            >
              <div class="d-flex mt-8">
                <v-text-field
                  outlined
                  solo
                  flat
                  label="Your email address"
                  hide-details
                  class=" rounded-r-0"
                ></v-text-field>

                <v-btn
                  class="primary rounded-l-0 text-capitalize"
                  x-large
                  height="56"
                >
                  Subscribe
                </v-btn>
              </div>
            </InfoCard>
          </v-col>

          <v-col cols="12" md="6" lg="5">
            <info-card
              title="Newsletter"
              subtitle="Duis aute irure dolor in reprehenderit in voluptate velit
                      esse cillum dolore."
              dark
              color="#30353c"
              class="pa-10"
            >
              <div class="d-flex mt-8">
                <v-btn
                  class="primary rounded-l-0 text-capitalize"
                  x-large
                  height="56"
                >
                  View All Infos
                </v-btn>
              </div>
            </info-card>
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>

    <v-sheet light class="py-16">
      <v-container>
        <div>
          <v-row justify="space-around" align="center" no-gutters>
            <v-col lg="11">
              <div class="primary--text text-h3 font-weight-bold">
                Latest Posts
              </div>

              <v-row>
                <v-col
                  cols="12"
                  md="6"
                  lg="4"
                  v-for="item in 15"
                  :key="item"
                  class="py-12"
                >
                  <simple-card
                    image="https://cdn.pixabay.com/photo/2021/01/30/18/07/salzburg-5964812_1280.jpg"
                    category="News"
                    date="February 3rd, 2021"
                    title="Ut enim blandit volutpat maecenas volutpat blandit"
                    category-class="deep-purple white--text"
                    flat
                    color="transparent"
                  />
                </v-col>
              </v-row>
            </v-col>
          </v-row>
        </div>
      </v-container>
    </v-sheet>
  </div>
</template>
<script>
import SimpleCard from "@/components/Cards/SimpleCard";
import InfoCard from "@/components/Cards/InfoCard";
import Header from "@/components/Layouts/Home/Header";
export default {
  components: { Header, InfoCard, SimpleCard }
};
</script>
