<script>
export default {
  props: {
    value: String
  },
  compute: {
    dataValue: {
      get() {
        return this.value;
      }
    }
  }
  watch: {
    dataValue{
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
