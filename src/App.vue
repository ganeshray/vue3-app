<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <v-toolbar-title>My Vuetify App</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn to="/" text>
        Home
      </v-btn>
      <v-btn to="/about" text>
        About
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>

    <v-footer app color="primary" dark>
      <span class="white--text">© 2024</span>
    </v-footer>
  </v-app>
</template>