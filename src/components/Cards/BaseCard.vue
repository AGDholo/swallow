<template>
  <v-card v-bind="$attrs">
    <slot />
  </v-card>
</template>

<script>
export default {
  name: "BaseCard"
};
</script>

<style scoped></style>
