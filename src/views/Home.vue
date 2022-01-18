<template>
  <div>
    <Nav></Nav>
    <v-container>
    <v-row 
        style="height: 150px;">
      <v-col
        cols="12"
        sm="4"
          v-for="(personaje, index) in Personajes"
          :key="index"
      >
          <Card :Character="personaje"></Card>
      </v-col>
    </v-row>
  </v-container>
  <Footer></Footer>
  </div>
</template>

<script>
import Nav from '../components/Nav.vue'
import Card from '../components/Card.vue'
import Footer from '../components/Footer.vue'

import Personajes from "../../personajes.js";
export default {

  data() {
    return {
      Personajes: Personajes
    }
  },
  components: {
    Nav, Card, Footer
  }
}
</script>

<style scoped>
</style>