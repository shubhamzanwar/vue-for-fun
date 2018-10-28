<script>
export default {
  props: {
    label: String,
    value: String
  }
};
</script>

<template>
  <label>
    <div>{{ label }}</div>

    <input
      type="text"
      data-test="input"
      :value="value"
      @input="$emit('input', $event.target.value)"
    >
  </label>
</template>

<style>
</style>
