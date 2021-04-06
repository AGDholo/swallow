<template>
  <v-app>
    <Appbar />

    <v-main>
      <router-view />
    </v-main>

    <Footer />
  </v-app>
</template>

<script>
import Footer from "@/components/Layouts/Footer";
export default {
  name: "App",

  components: {
    Footer,
    Appbar: () => import("./components/Layouts/Appbar")
  },

  data: () => ({
    //
  })
};
</script>
