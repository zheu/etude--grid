<script>
export default {
  render(h) {
    return <tr>{this.$scopedSlots.default({})}</tr>;
  }
};
</script>
