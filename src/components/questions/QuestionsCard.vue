<template>
  <v-card max-width="750" elevation="10">
    <v-card-title class="pb-2" v-if="title">
      <v-icon
              color="blue"
              small
              left
      >
        {{ icon }}
      </v-icon>
      <span class="blue--text caption font-weight-light">{{ title }}</span>
    </v-card-title>
    <v-divider v-if="divider && title"></v-divider>
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
      <v-divider v-if="divider"></v-divider>
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
</template>

<script>
    export default {
        name: "QuestionSuggestions",
        props: {
            title: [String, Boolean],
            icon: String,
            divider: Boolean
        }
    }
</script>

<style scoped>

</style>