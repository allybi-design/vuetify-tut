<template>
  <nav color="dark accent-4" dark>
    <v-toolbar dark>
      <v-app-bar-nav-icon
        @click="isDrawOpen = !isDrawOpen"
      ></v-app-bar-nav-icon>

      <v-spacer />

      <v-img
        src="../assets/images/sandhills-global-logo.png"
        max-height="48"
        contain
      ></v-img>

      <v-spacer />

      <span>
        <v-icon left>fas fa-user</v-icon>
      </span>

      <span class="font-weight-light">
        Sign Out
        <v-icon>fas fa-sign-out-alt</v-icon>
      </span>
    </v-toolbar>

    <v-navigation-drawer absolute temporary dark v-model="isDrawOpen">
      <v-list-item>
        <v-img
          src="../assets/images/sandhills-global-logo.png"
          max-height="72"
          class="my-5"
          contain
        ></v-img>
      </v-list-item>
      <v-divider />
      <v-list dense>
        <v-list-item v-for="(item, index) in menuItems" :key="index" link>
          <v-list-item-content>
            <v-list-item-title>
              <h2 class="font-weight-light">{{ item }}</h2>
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {
  name: "navbar",
  data() {
    return {
      isDrawOpen: false,
      menuItems: [
        "About Us",
        "Brands",
        "Locations",
        "News",
        "Careers",
        "Contact Us"
      ]
    };
  }
};
</script>
