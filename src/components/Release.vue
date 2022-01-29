<template>
  <v-card class="rounded-lg pa-2" color="#0F0A1E">
    <v-row>
      <v-col cols="12" sm="6">
        <v-toolbar color="rgba(0,0,0,0)" flat dark class="py-4">
          <v-toolbar-title class="mt-n10">
            <span class="caption">Top Releases</span>
          </v-toolbar-title>
        </v-toolbar>
        <v-divider color="grey" class="mx-6 mt-3 mb-2"></v-divider>
        <v-list subheader two-line class="" flat color="rgba(0,0,0,0)" dark>
          <v-list-item class="py-n8">
            <span class="mr-2 caption">01</span>
            <v-list-item-avatar class="mr-2" rounded>
              <v-img src="1.jpg" />
            </v-list-item-avatar>
            <v-list-item-content>
              <v-list-item-title>Who Cares</v-list-item-title>
              <v-list-item-subtitle class="caption"
                >93k plays</v-list-item-subtitle
              >
            </v-list-item-content>
            <v-list-item-action>
              <v-btn icon>
                <v-icon color="grey lighten-1" small
                  >fas fa-chevron-right</v-icon
                >
              </v-btn>
            </v-list-item-action>
          </v-list-item>
          <v-divider color="grey" class="mx-6"></v-divider>
          <v-list-item>
            <v-icon small color="#C3F942" class="mr-2"
              >fas fa-headphones-alt</v-icon
            >
            <v-list-item-avatar class="mr-2" rounded>
              <v-img src="2.jpg" />
            </v-list-item-avatar>
            <v-list-item-content>
              <v-list-item-title>Miss You</v-list-item-title>
              <v-list-item-subtitle class="caption"
                >64k plays</v-list-item-subtitle
              >
            </v-list-item-content>
            <v-list-item-action>
              <v-btn icon>
                <v-icon color="grey lighten-1" small
                  >fas fa-chevron-right</v-icon
                >
              </v-btn>
            </v-list-item-action>
          </v-list-item>

          <v-divider color="grey" class="mx-6"></v-divider>
          <v-list-item>
            <span class="mr-2 caption">03</span>
            <v-list-item-avatar class="mr-2" rounded>
              <v-img src="3.jpg" />
            </v-list-item-avatar>
            <v-list-item-content>
              <v-list-item-title>WorldWide</v-list-item-title>
              <v-list-item-subtitle class="caption"
                >59k plays</v-list-item-subtitle
              >
            </v-list-item-content>
            <v-list-item-action>
              <v-btn icon>
                <v-icon color="grey lighten-1" small
                  >fas fa-chevron-right</v-icon
                >
              </v-btn>
            </v-list-item-action>
          </v-list-item>

          <v-divider color="grey" class="mx-6 mb-2"></v-divider>
        </v-list>
      </v-col>
      <v-col cols="12" sm="6">
        <v-toolbar color="rgba(0,0,0,0)" flat class="py-4">
          <v-spacer></v-spacer>
          <v-toolbar-title class="mt-n10">
            <span class="caption lime--text">ALL Releases</span>
          </v-toolbar-title>
          <v-btn class="mt-n8 ml-2" small color="#C3F942">
            + New Release
          </v-btn>
        </v-toolbar>
        <v-divider color="grey" class="mx-6 mt-3 mb-2"></v-divider>
        <v-list subheader two-line class="" flat color="rgba(0,0,0,0)" dark>
          <v-list-item class="py-n8">
            <span class="mr-2 caption">04</span>
            <v-list-item-avatar class="mr-2" rounded>
              <v-img src="4.jpg" />
            </v-list-item-avatar>
            <v-list-item-content>
              <v-list-item-title>Like Me</v-list-item-title>
              <v-list-item-subtitle class="caption"
                >21k plays</v-list-item-subtitle
              >
            </v-list-item-content>
            <v-list-item-action>
              <v-btn icon>
                <v-icon color="grey lighten-1" small
                  >fas fa-chevron-right</v-icon
                >
              </v-btn>
            </v-list-item-action>
          </v-list-item>
          <v-divider color="grey" class="mx-6"></v-divider>
          <v-list-item>
            <span class="mr-2 caption">05</span>
            <v-list-item-avatar class="mr-2" rounded>
              <v-img src="5.jpg" />
            </v-list-item-avatar>
            <v-list-item-content>
              <v-list-item-title>No Surprise</v-list-item-title>
              <v-list-item-subtitle class="caption"
                >23k plays</v-list-item-subtitle
              >
            </v-list-item-content>
            <v-list-item-action>
              <v-btn icon>
                <v-icon color="grey lighten-1" small
                  >fas fa-chevron-right</v-icon
                >
              </v-btn>
            </v-list-item-action>
          </v-list-item>

          <v-divider color="grey" class="mx-6"></v-divider>
          <v-list-item>
            <span class="mr-2 caption">06</span>
            <v-list-item-avatar class="mr-2" rounded>
              <v-img src="7.jpg" />
            </v-list-item-avatar>
            <v-list-item-content>
              <v-list-item-title>Each Time</v-list-item-title>
              <v-list-item-subtitle class="caption"
                >12k plays</v-list-item-subtitle
              >
            </v-list-item-content>
            <v-list-item-action>
              <v-btn icon>
                <v-icon color="grey lighten-1" small
                  >fas fa-chevron-right</v-icon
                >
              </v-btn>
            </v-list-item-action>
          </v-list-item>

          <v-divider color="grey" class="mx-6 mb-4"></v-divider>
        </v-list>
      </v-col>
    </v-row>
  </v-card>
</template>

<script>
export default {};
</script>

<style>
</style>