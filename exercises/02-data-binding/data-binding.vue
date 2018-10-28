<script>
export default {
  data() {
    return {
      name: "John",
      a: 0.1,
      b: 0.2,
      classNames: ["content"]
    };
  }
};
</script>

<template>
  <div v-bind:class="classNames">
    <h1>Hello {{name}}!</h1>

    <p data-test="expr">a + b = {{a + b}}</p>
  </div>
</template>

<style>
.content {
  color: crimson;
}
</style>
