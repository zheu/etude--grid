<template>
  <div id="app">
    <Grid v-bind="{ items }">
      <GridHeaders slot="headers" slot-scope="{ bindings, events }" v-bind="bindings" v-on="events">
        <template slot-scope="{}">
          <th>2</th>
          <th>3</th>
          <th>4</th>
        </template>
      </GridHeaders>
      <GridColumns slot="columns" slot-scope="{ bindings, events }" v-bind="bindings" v-on="events">
        <template slot-scope="{}">
          <td>2</td>
          <td>3</td>
          <td>4</td>
        </template>
      </GridColumns>
    </Grid>
  </div>
</template>

<script>
import Grid from "./components/Grid";
import GridColumns from "./components/GridColumns";
import GridRows from "./components/GridRows";
import GridHeaders from "./components/GridHeaders";

export default {
  name: "App",
  components: { Grid, GridColumns, GridHeaders, GridRows },
  data: () => ({
    items: [1, 2, 3, 4, 5]
  })
};
</script>

<style>
</style>
