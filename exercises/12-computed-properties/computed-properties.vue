<script>
export default {
  props: {
    firstName: String,
    lastName: String
  },
  computed: {
    name: {
      get() {
        return `${this.firstName} ${this.lastName}`;
      },
      set(newValue) {
        const [firstName, lastName] = newValue.split(" ");
        firstName !== this.firstName &&
          this.$emit("update:firstName", firstName);
        lastName !== this.lastName && this.$emit("update:lastName", lastName);
      }
    }
  },
  render() {
    return null;
  }
};
</script>
