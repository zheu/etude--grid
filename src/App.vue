<template>
  <div id="app">
    <Grid>
      <GridHeaders slot="headers" slot-scope="{ bindings, events }" v-bind="bindings" v-on="events"></GridHeaders>
      <GridColumns slot="columns" slot-scope="{ bindings, events }" v-bind="bindings" v-on="events"></GridColumns>
    </Grid>
  </div>
</template>

<script>
import Grid from "./components/Grid";
import GridColumns from "./components/GridColumns";
import GridHeaders from "./components/GridHeaders";

export default {
  name: "App",
  components: { Grid, GridColumns, GridHeaders }
};
</script>

<style>
</style>
