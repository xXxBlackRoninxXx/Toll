<template>
  <v-toolbar color="grey darken-3">
    <v-toolbar-side-icon color="white" @click.stop="drawer = !drawer"></v-toolbar-side-icon>
    <router-link to="/">
       <v-toolbar-title class="blue--text">Какой-то сайт</v-toolbar-title>
    </router-link>
      <v-spacer></v-spacer>
    <div class="hidden-sm-and-down">
      <v-btn color="blue">
        <v-icon color="white">build</v-icon>
      </v-btn>
      <router-link to="/contact" class="link">
      <v-btn color="blue" class="white--text">Контакты</v-btn>
      </router-link>
      <router-link to="/login">
      <v-btn color="blue" class="white--text">Logine</v-btn>
      </router-link>
    </div>
    <div class="hidden-md-and-up">

          <v-navigation-drawer temporary v-model="drawer" absolute height="400px">
            <v-list class="pa-1">
              <v-list-tile avatar>
                <v-list-tile-avatar>
                  <img src="https://pp.userapi.com/c846420/v846420709/d4867/XJ8XGT4EwOk.jpg">
                </v-list-tile-avatar>

                <v-list-tile-content>
                  <v-list-tile-title>Роман Ермилец</v-list-tile-title>
                </v-list-tile-content>
              </v-list-tile>
            </v-list>

            <v-list class="pt-0" dense>
              <v-divider></v-divider>

              <v-list-tile
                v-for="item in items" :key="item.title">
                <v-list-tile-action>
                  <v-icon>{{ item.icon }}</v-icon>
                </v-list-tile-action>

                <v-list-tile-content>
                  <v-list-tile-title>{{ item.title }}</v-list-tile-title>
                </v-list-tile-content>
              </v-list-tile>
            </v-list>
          </v-navigation-drawer>
    </div>
  </v-toolbar>
</template>

<script>
  export  default {
    data() {
      return {
        drawer: null,
        items: [
          {title: 'Home', icon: 'dashboard'},
          {title: 'About', icon: 'question_answer'}
        ]
      }
    }
  }
</script>

<style>
  .link :active{
    text-decoration: none !important;
  }
</style>
