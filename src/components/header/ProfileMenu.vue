<template>
  <v-menu
          close-on-content-click
          bottom
          offset-y
          transition="slide-y-transition"
          nudge-bottom="16"
  >
    <template v-slot:activator="{ on }">
      <div v-on="on" style="cursor: pointer">
        <v-avatar color="teal" size="40">
          <span class="white--text">BW</span>
        </v-avatar>
        <v-icon>mdi-chevron-down</v-icon>
      </div>
    </template>

    <v-card width="220">
      <v-list dense class="pa-0">
        <v-list-item-group>
          <v-list-item>
            <v-list-item-avatar>
              <v-avatar color="teal" size="40">
                <span class="white--text">BW</span>
              </v-avatar>
            </v-list-item-avatar>

            <v-list-item-content>
              <v-list-item-title>Bruce Willis</v-list-item-title>
              <v-list-item-subtitle>View Profile</v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>
        </v-list-item-group>
        <v-list-item-group>
          <v-list-item>
            <v-list-item-icon>
              <v-icon class="pa-2">mdi-settings</v-icon>
            </v-list-item-icon>
            <v-list-item-content class="ms-n4">
              <v-list-item-title>Settings</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-icon>
              <v-icon class="pa-2">mdi-account-plus</v-icon>
            </v-list-item-icon>
            <v-list-item-content class="ms-n4">
              <v-list-item-title>Invite</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-icon>
              <v-icon class="pa-2">mdi-power</v-icon>
            </v-list-item-icon>
            <v-list-item-content class="ms-n4">
              <v-list-item-title>Sign out</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-card>
  </v-menu>
</template>

<script>
    export default {
        name: "ProfileMenu"
    }
</script>

<style scoped>

</style>