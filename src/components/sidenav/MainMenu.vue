<template>
  <v-list dense>
    <v-list-item link to="/" color="primary" :ripple="false">
      <v-list-item-action>
        <v-icon>mdi-home</v-icon>
      </v-list-item-action>
      <v-list-item-content>
        <v-list-item-title class="body-2 font-weight-regular">Home</v-list-item-title>
      </v-list-item-content>
    </v-list-item>
    <v-list-item link to="/feed" color="primary" :ripple="false">
      <v-list-item-action>
        <v-icon>mdi-view-stream</v-icon>
      </v-list-item-action>
      <v-list-item-content>
        <v-list-item-title class="body-2 font-weight-regular">Feed</v-list-item-title>
      </v-list-item-content>
    </v-list-item>
    <v-list-item link color="primary" :ripple="false">
      <v-list-item-action>
        <v-icon>mdi-account-group</v-icon>
      </v-list-item-action>
      <v-list-item-content>
        <v-list-item-title class="body-2 font-weight-regular">Experts</v-list-item-title>
      </v-list-item-content>
    </v-list-item>
    <v-list-item link color="primary" :ripple="false">
      <v-list-item-action>
        <v-icon>mdi-chart-timeline-variant</v-icon>
      </v-list-item-action>
      <v-list-item-content>
        <v-list-item-title class="body-2 font-weight-regular">Dashboard</v-list-item-title>
      </v-list-item-content>
    </v-list-item>
  </v-list>
</template>

<script>
    export default {
        name: "MainMenu"
    }
</script>

<style scoped>
  .v-list-item {
    border-left: solid 4px transparent;
  }
  .v-list-item--active {
    border-left: solid 4px;
  }
</style>