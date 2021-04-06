<template>
  <base-card v-bind="$attrs">
    <div>
      <div class="primary--text text-h4 font-weight-bold">
        {{ title }}
      </div>

      <div class="text-h6 my-1">
        <v-row>
          <v-col cols="12" md="10" lg="8">
            {{ subtitle }}
          </v-col>
        </v-row>
      </div>

      <slot />
    </div>
  </base-card>
</template>

<script>
import BaseCard from "@/components/Cards/BaseCard";
export default {
  name: "InfoCard",
  components: { BaseCard },
  props: {
    title: {
      type: String
    },
    subtitle: {
      type: String
    }
  }
};
</script>

<style scoped></style>
