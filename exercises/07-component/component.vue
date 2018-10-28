<script>
import MyComponent from "./my-component.vue";

export default {
  components: {
    MyComponent
  },
  data() {
    return {
      name: "Shubham"
    };
  }
};
</script>

<template>
  <div class="component-composition">
    <my-component :name="name" />
  </div>
</template>

<style>
</style>
