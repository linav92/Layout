<template>
  <div>
    <v-card class="my-4" max-width="344">
      <v-img :src="Character.imagen" height="200px"></v-img>
      <v-card-title>{{ Character.nombre }}</v-card-title>
    </v-card>
  </div>
</template>
<script>
export default {
  props: ["Character"],
};
</script>

<style scoped>
.v-card {
  margin: 0 auto;
}
</style>