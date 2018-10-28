<script>
export default {
  data() {
    return {
      person: {
        firstName: "John",
        lastName: "Doe",
        age: 30
      },
      fruits: ["Apple", "Mango"],
      range: 4
    };
  }
};
</script>

<template>
  <div class="iterative-rendering">
    <div data-test="fruits">
      <!-- render items from fruits here -->
      <div data-test="item" v-for="fruit in fruits" :key="fruit">{{fruit}}</div>
    </div>

    <div data-test="person">
      <!-- render properties from person here -->
      <div data-test="property" v-for="(value, key) in person">{{key}}: {{value}}</div>
    </div>

    <div data-test="range">
      <!-- render range here -->
      <div data-test="item" v-for="item in range"></div>
    </div>
  </div>
</template>

<style>
</style>
