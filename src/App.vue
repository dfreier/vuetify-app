<template>
  <v-app class="grey">
    <v-navigation-drawer
            floating
            app
            mobile-break-point="960"
            class="elevation-8"
            :value="opened"
            @input="opened = $event"
    >
      <div class="px-6 py-3" style="display: flex; justify-content: space-between; align-items: center">
        <v-avatar color="teal" style="border-radius: 2px" tile size="40">
          <span class="white--text">ST</span>
        </v-avatar>
        <span class="subtitle-1">Network</span>
        <v-btn depressed color="gray" small :ripple="false">
          <v-icon>mdi-menu-down</v-icon>
        </v-btn>
      </div>
     <div class="px-6 py-4 d-flex" >
       <v-btn class="flex-grow-1" depressed color="primary">
         <v-icon left>mdi-plus</v-icon> Ask
       </v-btn>
     </div>
      <v-list dense nav>
        <v-list-item link>
          <v-list-item-action>
            <v-icon>mdi-home</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link>
          <v-list-item-action>
            <v-icon>mdi-view-stream</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Feed</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
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

      <div>
        <v-avatar color="teal" size="40">
          <span class="white--text">BW</span>
        </v-avatar>
        <v-icon>mdi-menu-down</v-icon>
      </div>
    </v-app-bar>

    <v-content color="gray" >
      <HelloWorld />
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

        <v-btn value="nearby" @click="opened = true">
          <span>More</span>
          <v-icon>mdi-dots-horizontal</v-icon>
        </v-btn>
      </v-bottom-navigation>
    </v-content>

  </v-app>
</template>

<script>
    import HelloWorld from './components/HelloWorld';

    export default {
        name: 'App',

        components: {
            HelloWorld,
        },

        data: () => ({
            opened: true
        }),
    };
</script>
