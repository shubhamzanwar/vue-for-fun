<script>
export default {
  methods: {
    handleClick() {},
    handleMouseDown() {}
  }
};
</script>

<template>
  <div class="event-binding">
    <input
      type="text"
      data-test="input"
      v-on:click="handleClick"
      v-on:mousedown="(e) => handleMouseDown()"
    />
  </div>
</template>

<style>
</style>
