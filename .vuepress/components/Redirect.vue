<script>
/** Redirects to the given 'to' url, which is relative to the current location. */
export default {
  name: 'Redirect',
  props: {
    to: {
      type: String,
      required: true
    }
  },
  beforeCreate() {
    this.$router.replace(this.to)
  }
}
</script>