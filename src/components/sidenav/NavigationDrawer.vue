<template>
  <v-navigation-drawer
          floating
          app
          mobile-break-point="960"
          class="elevation-8"
          width="240"
  >
    <NetworkSelector></NetworkSelector>
    <AskButton></AskButton>
    <MainMenu></MainMenu>
  </v-navigation-drawer>
</template>

<script>
    import NetworkSelector from "./NetworkSelector";
    import AskButton from "./AskButton";
    import MainMenu from "./MainMenu";

    export default {
        name: "NavigationDrawer",
        components: {
            NetworkSelector,
            AskButton,
            MainMenu
        }
    }
</script>

<style scoped>

</style>