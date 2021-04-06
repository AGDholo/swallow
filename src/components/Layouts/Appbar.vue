<template>
  <v-app-bar
    app
    color="#141618"
    dark
    height="84"
    elevation="4"
    elevate-on-scroll
  >
    <v-container class="d-flex align-center justify-space-between">
      <div class="d-flex align-center">
        <router-link to="/">
          <v-toolbar-title
            class="text-h4 primary--text d-flex align-center font-weight-bold"
          >
            <v-avatar> <v-img src="../../assets/swallow.svg"></v-img></v-avatar>
            Swallow
          </v-toolbar-title></router-link
        >
        <div class="ml-4">
          <v-btn
            link
            text
            v-for="item in leftItems"
            :key="item.title"
            :to="item.to"
            class="text-capitalize text-h6 font-weight-regular ml-1"
            large
            exact
          >
            {{ item.title }}
          </v-btn>
        </div>
      </div>

      <div class="d-flex align-center">
        <v-btn
          link
          text
          v-for="item in rightItems"
          :key="item.title"
          :to="item.to"
          :href="item.href"
          :target="item.href ? '_black' : ''"
          class="text-capitalize font-weight-regular mr-1"
          exact
        >
          {{ item.title }}
        </v-btn>

        <v-text-field
          outlined
          solo
          flat
          label="Search"
          prepend-inner-icon="mdi-magnify"
          dense
          hide-details
        ></v-text-field>
      </div>
    </v-container>
  </v-app-bar>
</template>

<script>
export default {
  data() {
    return {
      leftItems: [
        { title: "Category", to: "/category" },
        { title: "Detail", to: "/detail" },
        { title: "Newsletter", to: "/newsletter" }
      ],
      rightItems: [{ title: "Free Download", href: "https://github.com" }]
    };
  }
};
</script>

<style lang="scss">
a {
  text-decoration: none;
}
</style>
