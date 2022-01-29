<template>
  <v-card class="rounded-lg" color="#0F0A1E">
    <v-toolbar color="rgba(0,0,0,0)" flat dark class="py-4">
      <v-toolbar-title class="mt-n5">
        <span class="caption">Streams</span><br />450,210
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <div style="text-align: center">
        <v-avatar size="40px">
          <v-img src="all.png" /> </v-avatar
        ><br />
        <span class="caption">ALL</span>
      </div>

      <div style="text-align: center; margin-left: 60px">
        <v-avatar size="40px">
          <v-img src="spotify.png" /> </v-avatar
        ><br />
        <span class="caption">Spotify</span>
      </div>
      <div style="text-align: center; margin-left: 60px">
        <v-avatar size="40px">
          <v-img src="youtube.png" /> </v-avatar
        ><br />
        <span class="caption">YouTube</span>
      </div>
      <div style="text-align: center; margin-left: 60px">
        <v-avatar size="40px">
          <v-img src="music.png" /> </v-avatar
        ><br />
        <span class="caption">Apple Music</span>
      </div>
      <div style="text-align: center; margin-left: 40px">
        <v-icon color="#C3F942"> fas fa-arrow-right </v-icon><br />
        <v-icon color="grey" class="mt-2"> fas fa-arrow-left </v-icon>
      </div>
    </v-toolbar>
    <div class="mt-5">
      <line-chart
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
../chart/LineChart.js
<script>
import LineChart from "../chart/LineChart.js";
export default {
  name: "Home",
  data: () => ({}),
  components: {
    LineChart,
  },
  props: {
    chartId: {
      type: String,
      default: "line-chart",
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

