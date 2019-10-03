<template>
  <v-app app class="amber darken-4">
    <Navbar />
    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
export default {
  name: "App",
  components: {
    Navbar: require("./components/Navbar.vue").default
  },
  data: () => ({
    //
  })
};
</script>
