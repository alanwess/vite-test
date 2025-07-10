<template>
  <v-app>
    <v-app-bar color="#054ADA" dark>
      <v-toolbar-title @click="goHome" style="cursor: pointer;"><v-icon class="mr-2">mdi-book</v-icon> Books
        Frontend</v-toolbar-title>
      <v-spacer />
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>

    <v-footer color="#054ADA" dark app>
      <v-col class="text-center white--text">Books Frontend</v-col>
    </v-footer>
  </v-app>
</template>

<script setup lang="ts">
import { useRouter } from 'vue-router'
const router = useRouter()
const goHome = () => router.push('/')
</script>
