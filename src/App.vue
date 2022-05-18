<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
      dense
    >
      <v-spacer></v-spacer>
    </v-app-bar>

    <v-main>
      <card-loop></card-loop>
    </v-main>
  </v-app>
</template>

<script>
import CardLoop from "./components/CardLoop.vue";

export default {
  name: 'App',

  components: {
    CardLoop,
  },

  data: () => ({
    //
  }),
};
</script>
