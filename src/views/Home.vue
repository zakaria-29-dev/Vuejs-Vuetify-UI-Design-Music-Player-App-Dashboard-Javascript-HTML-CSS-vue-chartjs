<template>
  <v-app :style="{background: $vuetify.theme.themes.dark.background}">
    <SideBar />
    <RightSideBar />
    <Dashboard />
  </v-app>
</template>

<script>
  import SideBar from '../components/SideBar'
  import RightSideBar from '../components/RightSideBar'
  import Dashboard from '../components/Dashboard'

  export default {
    name: 'Home',

    components: {
      SideBar,
      RightSideBar,
      Dashboard
      
    },
  }
</script>
