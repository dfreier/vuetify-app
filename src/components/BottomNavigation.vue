<template>
  <v-bottom-navigation class="d-flex d-md-none" app grow>
    <v-btn value="recent">
      <span>Feed</span>
      <v-icon>mdi-view-stream</v-icon>
    </v-btn>

    <v-btn value="favorites">
      <span>Experts</span>
      <v-icon>mdi-account-group</v-icon>
    </v-btn>

    <v-btn value="favorites">
      <span>Ask</span>
      <v-icon>mdi-plus</v-icon>
    </v-btn>

    <v-btn value="nearby">
      <span>Nots</span>
      <v-icon>mdi-bell</v-icon>
    </v-btn>

    <v-btn value="nearby">
      <span>More</span>
      <v-icon>mdi-dots-horizontal</v-icon>
    </v-btn>
  </v-bottom-navigation>
</template>

<script>
    export default {
        name: "BottomNavigation"
    }
</script>

<style scoped>

</style>