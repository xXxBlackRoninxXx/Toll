<template>
  <v-toolbar color="grey darken-3">
    <v-toolbar-side-icon color="white"></v-toolbar-side-icon>
    <v-toolbar-title class="blue--text">Какой-то сайт</v-toolbar-title>
      <v-spacer></v-spacer>
    <div class="hidden-sm-and-down">
      <v-btn color="blue">
        <v-icon color="white">build</v-icon>
      </v-btn>
      <v-btn flat></v-btn>
      <router-link to="/login">
      <v-btn color="blue" class="white--text">Logine</v-btn>
      </router-link>
    </div>
  </v-toolbar>
</template>
