<script>
export default {
  props: {
    items: Array
  },

  render(h) {
    const headers = this.$scopedSlots.headers({});
    const columns = this.$scopedSlots.columns({});
    const rows = this.items.map(row => <tr>{columns}</tr>);

    return (
      <table>
        <thead>{headers}</thead>
        <tbody>{rows}</tbody>
      </table>
    );
  }
};
</script>

