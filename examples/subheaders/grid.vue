<template>
  <v-layout row>
    <v-flex xs12 sm6 offset-sm3>
      <v-card>
        <v-toolbar class="white elevation-0">
          <v-btn icon light>
            <v-icon class="grey--text text--darken-2">arrow_back</v-icon>
          </v-btn>
          <v-toolbar-title class="grey--text text--darken-4">Albums</v-toolbar-title>
          <v-spacer></v-spacer>
          <v-btn icon light>
            <v-icon class="grey--text text--darken-2">search</v-icon>
          </v-btn>
        </v-toolbar>
        <v-subheader>May</v-subheader>
        <v-container fluid grid-list-xs>
          <v-layout row wrap>
            <v-flex xs4 v-for="i in 6" :key="i">
              <img
                class="image"
                v-bind:src="`https://randomuser.me/api/portraits/men/${i + 20}.jpg`"
                alt="lorem"
                width="100%"
                height="100%"
              >
            </v-flex>
          </v-layout>
        </v-container>
        <v-subheader>June</v-subheader>
        <v-container fluid grid-list-xs>
          <v-layout row wrap>
            <v-flex xs4 v-for="i in 6" :key="i">
              <img class="image" v-bind:src="`https://randomuser.me/api/portraits/women/${i + 5}.jpg`" alt="lorem" width="100%" height="100%">
            </v-flex>
          </v-layout>
        </v-container>
        <v-footer class="mt-5"></v-footer>
      </v-card>
    </v-flex>
  </v-layout>
</template>
