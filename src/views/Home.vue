<template>
    <v-app :style="{ backgroundColor: bgColor }">
        <v-row justify="center" align="center">
            <v-spacer></v-spacer>
            <v-col>
                <v-row>
                    <img :src="logo"/>
                </v-row>
                <v-row justify="start" align="center" class="mt-10">
                    <v-spacer></v-spacer>
                    <v-btn elevation="0" x-large color="">Jouer</v-btn>
                    <v-spacer></v-spacer>
                </v-row>
            </v-col>
            <v-spacer></v-spacer>
        </v-row>
    </v-app>
</template>

<script>
import m from './model'
import logo from '../assets/quiestce.jpg'
export default {
  name: 'Home',
  data: () => m,
  created () {
    this.logo = logo
  }
}
</script>
