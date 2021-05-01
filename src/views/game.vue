<template>
    <v-app :style="{ backgroundColor: bgColor }">
        <v-app-bar fixed clipped-left dense color="#673AB7" elevation="0">
            epitech
            <v-spacer></v-spacer>
            cheatcode
        </v-app-bar>
        <v-row align="center" justify="center">
            <v-col>
                <v-container fluid grid-list-md>
                    <v-layout row wrap>
                        <v-flex v-for="char in characters" :key="char.name">
                            <v-card>
                                {{char.name}}
                            </v-card>
                        </v-flex>
                    </v-layout>
                </v-container>
            </v-col>
        </v-row>
    </v-app>
</template>

<script>
import m from './model'
import characters from '../../public/character_struct.json'
export default {
  name: 'Game',
  data: () => m,
  created () {
    this.characters = characters.characters
    console.log(this.characters)
  }
}
</script>
