<template>
  <v-app>
    <v-app-bar>
      <v-toolbar-title>Logo</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-app-bar-nav-icon
        class="d-md-none"
        @click="drawer = !drawer"
      ></v-app-bar-nav-icon>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" temporary>
      <ul>
        <li>menu</li>
      </ul>
    </v-navigation-drawer>

    <v-main class="bg-grey-lighten-2">
      <v-container>
        <NuxtPage />
      </v-container>
    </v-main>
  </v-app>
</template>
  
<script setup>
import { ref } from "vue";
const drawer = ref(null);
</script>