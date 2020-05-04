<template>
  <div class="px-6 py-3" style="display: flex; justify-content: space-between; align-items: center">
    <v-avatar color="teal" style="border-radius: 2px" tile size="40">
      <span class="white--text">ST</span>
    </v-avatar>
    <span class="subtitle-1">Network</span>
    <v-btn depressed color="gray" small :ripple="false" class="pa-0" min-width="28">
      <v-icon>mdi-chevron-down</v-icon>
    </v-btn>
  </div>
</template>

<script>
    export default {
        name: "NetworkSelector"
    }
</script>

<style scoped>

</style>