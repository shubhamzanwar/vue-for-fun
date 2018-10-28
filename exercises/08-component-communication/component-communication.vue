<script>
export default {
  props: {
    title: {
      type: String
    }
  }
};
</script>

<template>
  <div class="component-communication">
    <h1>{{title}}</h1>

    <button @click="() => $emit('done')">Done</button>
  </div>
</template>

<style>
</style>
