<template>
  <v-card
    class="mx-auto"
    max-width="400"
  >
    <v-img
      class="white--text align-end"
      height="200px"
      src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
    >
      <v-card-title>HOME</v-card-title>
    </v-img>

    <v-card-subtitle class="pb-0">HOME</v-card-subtitle>

    <v-card-text class="text--primary">
      <div>HOME</div>
      {{$auth.$state.loggedIn}}
    </v-card-text>

    <v-card-actions>

      <v-btn
        color="orange"
        text
      >
        HOME
      </v-btn>

      <v-btn
        color="orange"
        text
      >
        HOME
      </v-btn>
    </v-card-actions>
  </v-card>

</template>

<script>
  export default {
    mounted() {

    }
  }
</script>

<style>

</style>
