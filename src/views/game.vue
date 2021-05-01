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
                                <img :src="char.sprite">
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
import alain from '../../public/characters/alain.jpg'
import ali from '../../public/characters/ali.jpg'
import amir from '../../public/characters/amir.jpg'
import christine from '../../public/characters/christine.jpg'
import diego from '../../public/characters/diego.jpg'
import hugo from '../../public/characters/hugo.jpg'
import ines from '../../public/characters/ines.jpg'
import jacques from '../../public/characters/jacques.jpg'
import julien from '../../public/characters/julien.jpg'
import laetitia from '../../public/characters/laetitia.jpg'
import leo from '../../public/characters/leo.jpg'
import liam from '../../public/characters/liam.jpg'
import lilou from '../../public/characters/lilou.jpg'
import mathieu from '../../public/characters/mathieu.jpg'
import mathis from '../../public/characters/mathis.jpg'
import nathan from '../../public/characters/nathan.jpg'
import noemie from '../../public/characters/noemie.jpg'
import pauline from '../../public/characters/pauline.jpg'
import sebastien from '../../public/characters/sebastien.jpg'
import sophie from '../../public/characters/sophie.jpg'
import stephane from '../../public/characters/stephane.jpg'
import thomas from '../../public/characters/thomas.jpg'
import banana from '../../public/characters/banana_anonymous.png'
import elliot from '../../public/characters/mr_robot.png'
export default {
  name: 'Game',
  data: () => m,
  created () {
    this.characters = characters.characters
    this.characters[0].sprite = alain
    this.characters[1].sprite = ali
    this.characters[2].sprite = amir
    this.characters[3].sprite = christine
    this.characters[4].sprite = diego
    this.characters[5].sprite = hugo
    this.characters[6].sprite = ines
    this.characters[7].sprite = jacques
    this.characters[8].sprite = julien
    this.characters[9].sprite = laetitia
    this.characters[10].sprite = leo
    this.characters[11].sprite = liam
    this.characters[12].sprite = lilou
    this.characters[13].sprite = mathieu
    this.characters[14].sprite = mathis
    this.characters[15].sprite = nathan
    this.characters[16].sprite = noemie
    this.characters[17].sprite = pauline
    this.characters[18].sprite = sebastien
    this.characters[19].sprite = sophie
    this.characters[20].sprite = stephane
    this.characters[21].sprite = thomas
    this.characters[22].sprite = banana
    this.characters[23].sprite = elliot
  }
}
</script>
