<script>
export default {};
</script>

<template>
  <div class="content-distribution">
    <div data-test="title">
      <slot name="title">
      This is title.
      </slot>
    </div>
    <slot />
  </div>
</template>

<style>
</style>
