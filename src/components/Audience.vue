<template>
  <v-card class="rounded-lg" color="#0F0A1E">
    <v-toolbar color="rgba(0,0,0,0)" flat dark class="py-4">
      <v-toolbar-title class="mt-n10">
        <span class="caption">Target Audience</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-icon color="#C3F942" small class="mt-n8">fas fa-ellipsis-h</v-icon>
    </v-toolbar>
    <div>
      <bar-chart
        :chart-id="chartId"
        :width="width"
        :height="height"
        :css-classes="cssClasses"
        :styles="styles"
        :plugins="plugins"
      />
    </div>
  </v-card>
</template>

<script>
import BarChart from "../chart/BarChart.js";
export default {
  name: "Home",
  data: () => ({}),
  components: {
    BarChart,
  },
  props: {
    chartId: {
      type: String,
      default: "bar-chart",
    },
    width: {
      type: Number,
      default: 400,
    },
    height: {
      type: Number,
      default: 230,
    },
    cssClasses: {
      default: "",
      type: String,
    },
    styles: {
      type: Object,
      default: () => {},
    },
    plugins: {
      type: Array,
      default: () => {},
    },
  },
};
</script>

