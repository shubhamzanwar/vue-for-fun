<script>
export default {
  props: {
    value: String
  },
  watch: {
    value: {
      handler(newValue, oldValue) {
        console.log(`value changed from ${oldValue} to ${newValue}`);
      },
      immediate: true
    }
  },
  render() {
    return null;
  }
};
</script>
