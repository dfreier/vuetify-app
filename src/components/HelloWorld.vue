<template>
  <div class="pa-2 px-sm-8 py-sm-4 ">
    <v-card max-width="750" elevation="10">
      <v-card-title class="pb-2">
        <v-icon
                color="blue"
                small
                left
        >
          mdi-star-four-points-outline
        </v-icon>
        <span class="blue--text caption font-weight-light">Questions for you</span>
      </v-card-title>
      <v-list three-line class="pt-0 pb-3">

        <v-list-item class="py-0" style="min-height: 64px" >
          <v-list-item-content class="py-2">
            <v-list-item-title class="body-2 font-weight-thin mb-2">Who many similar questions are shown normally?</v-list-item-title>
            <div class="d-flex align-content-space-between">
              <v-list-item-subtitle><span class="font-weight-bold caption pink--text">CMS</span> <span class="caption">bl alb al bla </span>
              </v-list-item-subtitle>
              <v-list-item-action class="ma-0 me-6 me-sm-2">
                <v-btn text small color="blue">Answer</v-btn>
              </v-list-item-action>
            </div>
          </v-list-item-content>

        </v-list-item>
        <v-list-item class="py-0"  style="min-height: 64px">
          <v-list-item-content class="py-2">
            <v-list-item-title class="body-2 font-weight-thin mb-2">Who is an expert in landscape photography?</v-list-item-title>
            <div class="d-flex align-content-space-between">
              <v-list-item-subtitle><span class="font-weight-bold caption teal--text">Art</span> <span class="caption">bl alb al bla </span>
              </v-list-item-subtitle>
              <v-list-item-action class="ma-0 me-6 me-sm-2">
                <v-btn text small color="blue">Answer</v-btn>
              </v-list-item-action>
            </div>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-card>

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
      <v-card-text>
        <div class="d-flex flex-column">
          <span class="caption font-weight-light">Top popular tags</span>
          <v-chip-group
                  multiple
                  column
          >
            <v-chip v-for="tag in tags" outlined :key="tag">
              {{ tag }}
            </v-chip>
          </v-chip-group>
        </div>
      </v-card-text>
    </v-card>
  </div>
</template>

<script>
    export default {
        name: 'HelloWorld',

        data: () => ({
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
        }),
    }
</script>
