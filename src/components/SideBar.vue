<template>
  <v-navigation-drawer
    v-model="drawer"
    app
    color="#0F0A1E"
    mini-variant
    mini-variant-width="90"
  >
    <v-avatar class="d-block text-center mx-auto mt-4" size="60">
      <v-icon color="#C3F942" x-large>fab fa-soundcloud</v-icon>
    </v-avatar>
    <v-list flat class="mt-16" dark>
      <v-list-item-group v-model="selectedItem">
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          active-class="border"
          v-slot="{ active }"
          :ripple="false"
        >
          <v-list-item-content>
            <v-icon
              v-text="item.icon"
              :color="active ? '#C3F942' : 'grey'"
            ></v-icon>
          </v-list-item-content>
        </v-list-item>
      </v-list-item-group>
    </v-list>
    <div
      style="
        position: absolute;
        bottom: 20px;
        margin-left: auto;
        margin-right: auto;
        left: 0;
        right: 0;
        text-align: center;
      "
    >
      <v-icon color="grey">far fa-question-circle</v-icon>
    </div>
  </v-navigation-drawer>
</template>

<script>
export default {
  data: () => ({
    selectedItem: 0,
    drawer: null,
    items: [
      { icon: "fas fa-podcast" },
      { icon: "fas fa-music" },
      { icon: "far fa-bell" },
      { icon: "fas fa-search-dollar" },
      { icon: "far fa-user" },
    ],
  }),
};
</script>

<style>
.border {
  text-decoration: none;
  text-shadow: 1px 1px 2px black, 0 0 15px #c3f942, 0 0 5px green;
}
.v-list-item-group .v-list-item--active {
  color: #c3f942 !important;
}
</style>