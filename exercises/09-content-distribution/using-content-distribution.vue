<script>
import MyComponent from "./content-distribution.vue";

export default {
  components: { MyComponent }
};
</script>

<template>
  <MyComponent>
    <template slot="title">
      title from parent.
    </template>
  </MyComponent>
</template>

<style>
</style>
