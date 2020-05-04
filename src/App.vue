<template>
  <v-app>
    <AppBar></AppBar>
    <NavigationDrawer></NavigationDrawer>
    <BottomNavigation></BottomNavigation>

    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
    import NavigationDrawer from "./components/sidenav/NavigationDrawer";
    import BottomNavigation from "./components/BottomNavigation";
    import AppBar from "./components/header/AppBar";

    export default {
        name: 'App',
        components: {
            NavigationDrawer,
            BottomNavigation,
            AppBar
        },
        data: () => ({
            opened: true
        })
    };
</script>
