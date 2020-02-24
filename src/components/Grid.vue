<script>
export default {
  render(h) {
    console.error("slots", this.$slots);
    console.error("scopedSlots", this.$scopedSlots);
    return h("div");
  }
};
</script>

