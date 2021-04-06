<template>
  <base-card v-bind="$attrs">
    <v-img class="rounded-lg" :src="image"></v-img>

    <div class="d-flex align-center my-3">
      <v-chip class="subtitle-2" :class="categoryClass" small>
        {{ category }}
      </v-chip>
      <div class="ml-2 body-2 grey--text text--lighten-1">
        {{ date }}
      </div>
    </div>

    <div class="text-h5 font-weight-bold">
      {{ title }}
    </div>
  </base-card>
</template>

<script>
import BaseCard from "@/components/Cards/BaseCard";
export default {
  name: "SimpleCard",
  components: { BaseCard },
  props: {
    image: {
      type: String
    },
    category: {
      type: String
    },
    date: {
      type: String
    },
    title: {
      type: String
    },
    categoryClass: {
      type: String,
      default: "deep-purple"
    }
  }
};
</script>

<style scoped></style>
