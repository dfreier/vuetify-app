<template>
  <v-card class="mt-2 mt-sm-4" max-width="750" elevation="10">
    <v-card-title class="pb-2">
      <v-icon
              color="blue"
              small
              left
      >
        mdi-flash
      </v-icon>
      <span class="blue--text caption font-weight-light">Subscribe to content</span>
    </v-card-title>
    <div class="d-flex flex-column flex-md-row">
      <v-card-text>
        <div class="d-flex flex-column">
          <span class="caption font-weight-light">Top popular tags</span>
          <v-chip-group
                  multiple
                  column
          >
            <v-chip v-for="tag in tags" outlined :key="tag" @click="snackbar = true">
              {{ tag }}
            </v-chip>
          </v-chip-group>
        </div>
      </v-card-text>
      <v-card-text >
        <div class="d-flex flex-column">
          <span class="caption font-weight-light">Top popular categories</span>
          <v-list dense flat>
            <v-list-item-group>
              <v-divider></v-divider>
              <v-list-item class="px-2" :ripple="false">
                <v-list-item-icon>
                  <v-icon x-small color="green">mdi-checkbox-blank-circle</v-icon>
                </v-list-item-icon>
                <v-list-item-content class="ms-n8">
                  <v-list-item-title class="caption font-weight-regular">IT Support</v-list-item-title>
                </v-list-item-content>
                <v-list-item-action class="my-0">
                  <v-btn color="blue" text small @click="snackbar = true">Subscribe</v-btn>
                </v-list-item-action>
              </v-list-item>
              <v-divider></v-divider>
              <v-list-item class="px-2" :ripple="false">
                <v-list-item-icon>
                  <v-icon x-small color="yellow">mdi-checkbox-blank-circle</v-icon>
                </v-list-item-icon>
                <v-list-item-content class="ms-n8">
                  <v-list-item-title class="caption font-weight-regular">Finance</v-list-item-title>
                </v-list-item-content>
                <v-list-item-action class="my-0">
                  <v-btn color="blue" text small @click="snackbar = true">Subscribe</v-btn>
                </v-list-item-action>
              </v-list-item>
              <v-divider></v-divider>
              <v-list-item class="px-2" :ripple="false">
                <v-list-item-icon>
                  <v-icon x-small color="orange">mdi-checkbox-blank-circle</v-icon>
                </v-list-item-icon>
                <v-list-item-content class="ms-n8">
                  <v-list-item-title class="caption font-weight-regular">HR</v-list-item-title>
                </v-list-item-content>
                <v-list-item-action class="my-0">
                  <v-btn color="blue" text small @click="snackbar = true">Subscribe</v-btn>
                </v-list-item-action>
              </v-list-item>
              <v-divider></v-divider>
            </v-list-item-group>
          </v-list>
        </div>
      </v-card-text>
    </div>
    <v-snackbar
            v-model="snackbar"
    >
      Subscribed
      <v-btn
              color="pink"
              text
              @click="snackbar = false"
      >
        Close
      </v-btn>
    </v-snackbar>
  </v-card>
</template>

<script>
    export default {
        name: "Subscriptions",
        data: () => ({
            snackbar: false,
            tags: [
                'Work',
                'Home Improvement',
                'Vacation',
                'Food',
                'Drawers',
                'Shopping',
                'Art',
                'Tech',
                'Creative Writing',
            ]
        })
    }
</script>

<style scoped>

</style>