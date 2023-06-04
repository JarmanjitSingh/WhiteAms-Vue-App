<script setup>
import { RouterView } from 'vue-router'
import Header from "./components/Header.vue"
import NavigationDrawer from "./components/NavigationDrawer.vue"
</script>

<template>
  <v-layout>
    <v-app-bar :elevation="5">
      <Header />
    </v-app-bar>
    <NavigationDrawer />
    
    <v-main style="min-height: 300px;">
      <RouterView />
    </v-main>
  </v-layout>
</template>

<style scoped></style>
