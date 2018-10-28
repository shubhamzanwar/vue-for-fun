<script>
import MyComponent from "./content-distribution.vue";

export default {
  components: { MyComponent }
};
</script>

<template>
  <MyComponent>
    <div slot="title">
      title from parent.
    </div>
  </MyComponent>
</template>

<style>
</style>
