<script>
export default {
  data() {
    return {
      timeOfDay: 8
    };
  }
};
</script>

<template>
  <div class="greet">
    <span v-if="timeOfDay < 10">Good Morning</span>
    <span v-else-if="timeOfDay < 17">Good Afternoon</span>
    <span v-else>Good Evening</span>
  </div>
</template>

<style>
</style>
