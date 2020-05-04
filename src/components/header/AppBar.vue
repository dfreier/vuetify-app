<template>
  <v-app-bar
          app
          elevation="5"
          color="white"
          height="64"
  >
    <v-autocomplete
            cache-items
            class="mx-4"
            flat
            hide-no-data
            hide-details
            label="Search..."
            prepend-icon="mdi-magnify"
            append-icon=""
            solo
    ></v-autocomplete>

    <v-spacer></v-spacer>
    <ProfileMenu></ProfileMenu>
  </v-app-bar>
</template>

<script>
  import ProfileMenu from "./ProfileMenu";
    export default {
        name: "AppBar",
        components: {
            ProfileMenu
        }
    }
</script>

<style scoped>

</style>