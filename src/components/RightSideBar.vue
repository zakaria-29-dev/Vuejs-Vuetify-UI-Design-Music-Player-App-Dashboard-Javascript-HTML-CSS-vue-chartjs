<template>
  <v-navigation-drawer app color="#0F0A1E" right width="260">
    <v-toolbar color="rgba(0,0,0,0)" flat class="d-flex justify-center">
      <v-avatar size="30" class="ml-n3">
        <v-img src="avatar.jpg"></v-img>
      </v-avatar>

      <v-btn text color="#7C7C7F" class="withoutupercase">AAE IdeaPro</v-btn>
      <v-btn icon dark class="ml-n3">
        <v-icon x-small color="#C3F942">fas fa-chevron-down</v-icon>
      </v-btn>
    </v-toolbar>
    <v-divider color="grey" class="mx-6"></v-divider>
    <v-row>
      <v-col cols="12" sm="6" class="pa-6">
        <strong class="ml-3 grey--text caption">Listeners Now</strong><br />
        <strong class="ml-3 white--text">1.186</strong>
      </v-col>
      <v-col cols="12" sm="6" class="pa-4 mt-3">
        <v-sparkline
          :value="value"
          :smooth="radius || false"
          :padding="padding"
          :line-width="width"
          :stroke-lineCap="lineCap"
          :fill="fill"
          :type="type"
          :auto-line-width="autoLineWidth"
          :color="color"
          :height="height"
          auto-draw
        >
        </v-sparkline> </v-col
      >>
    </v-row>
    <v-list subheader two-line dark>
      <v-list-item v-for="file in flags" :key="file.title">
        <v-list-item-avatar>
          <img :src="file.avatar" />
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title v-text="file.title"></v-list-item-title>
        </v-list-item-content>
        <v-list-item-action>
          <v-list-item-subtitle v-text="file.subtitle"></v-list-item-subtitle>
        </v-list-item-action>
      </v-list-item>
    </v-list>
    <v-divider color="grey" class="mx-6 mb-5"></v-divider>
    <v-card class="mx-5 rounded-xl" flat>
      <v-img height="300px" src="adel.jpg">
        <div
          style="
            position: absolute;
            bottom: 0px;
            margin-left: auto;
            margin-right: auto;
            left: 0px;
            right: 0px;
            text-align: center;
          "
        >
          <h5 class="white--text justify-center">Miss You</h5>
          <v-slider
            v-model="sld.val"
            :color="sld.color"
            track-color="white"
          ></v-slider>
          <v-card-text class="white--text d-flex justify-center">
            <v-list dark dense>
              <v-list-item>
                <v-list-item-icon>
                  <v-btn icon>
                    <v-icon class="ml-4">mdi-rewind</v-icon>
                  </v-btn>
                </v-list-item-icon>
                <v-list-item-icon>
                  <v-btn icon>
                    <v-icon class="">mdi-pause</v-icon>
                  </v-btn>
                </v-list-item-icon>
                <v-list-item-icon>
                  <v-btn icon>
                    <v-icon class="">mdi-fast-forward</v-icon>
                  </v-btn>
                </v-list-item-icon>
              </v-list-item>
            </v-list>
          </v-card-text>
        </div>
      </v-img>
    </v-card>
  </v-navigation-drawer>
</template>

<script>
export default {
  data: () => ({
    width: 5,
    radius: 10,
    padding: 8,
    lineCap: "round",
    value: [0, 2, 5, 9, 5, 10, 3, 5],
    fill: false,
    type: "trend",
    autoLineWidth: false,
    color: "#C3F942",
    height: 150,
    flags: [
      {
        avatar: "us.png",
        title: "United States",
        subtitle: "64%",
      },
      {
        avatar: "uk.png",
        title: "United Kingdom",
        subtitle: "12%",
      },
      {
        avatar: "ca.png",
        title: "Canada",
        subtitle: "9%",
      },
      {
        avatar: "au.png",
        title: "Australia",
        subtitle: "4%",
      },
    ],
    sld: {
      val: 25,
      color: "#C3F942",
    },
  }),
};
</script>

<style>
.v-btn.withoutupercase {
  text-transform: none !important;
}
.col-12 {
  padding: 5px !important;
}
.v-card__subtitle,
.v-card__text,
.v-card__title {
  padding: 0px !important;
}
.v-navigation-drawer .v-list:not(.v-select-list) {
  padding-top: 0px;
}
.v-list-item__avatar {
  margin-bottom: 0px !important;
  margin-top: 0px !important;
}
.v-list--two-line .v-list-item,
.v-list-item--two-line {
  min-height: 50px !important;
}
.v-messages {
  min-height: 0px !important;
}
</style>