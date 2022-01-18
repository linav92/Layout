<template>
  <div>
    <v-app-bar color="#BEE1E6">
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>Rick & Morty</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn elevation="0" color="#BEE1E6">Inicio</v-btn>
        <v-btn elevation="0" color="#BEE1E6">Buscar</v-btn>
        <v-btn elevation="0" color="#BEE1E6">Acerca de</v-btn>
      </v-toolbar-items>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" absolute left temporary color="#BEE1E6">
      <v-list nav dense>
        <v-list-item-group
          active-class="teal--text text--darken-4"
        >
          <v-list-item>
            <v-list-item-title color="#ffffff">Inicio</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Buscar</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Acerca de</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
  }),
};
</script>

<style scoped>
</style>
