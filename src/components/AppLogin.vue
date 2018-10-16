<template>
  <v-container>
  <v-form v-model="valid">
    <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="10"
      label="Name"
      required
    ></v-text-field>
    <v-text-field
      v-model="email"
      :rules="emailRules"
      label="E-mail"
      required
    ></v-text-field>
  </v-form>
  </v-container>
</template>

<script>
    export default {
        name: "AppLogin"
    }
</script>

<style scoped>

</style>
