<template>
  <v-container>
  <v-form @submit.prevent="submit">

    <v-text-field
      v-model="email"
      label="E-mail"
      required
    ></v-text-field>

    <v-text-field
      v-model="Password"
      :rules="Password"
      :counter="10"
      label="Пароль"
      type="password"
      required
    ></v-text-field>

    <v-btn class="green" type="submit" >Отправить</v-btn>
  </v-form>
  </v-container>
</template>

<script>
    export default {
        data(){
          return{
            email:null,
            password:null
          }
        },
      methods:{
          submit(){
            console.log('hello')
          }
      }
    }
</script>

<style scoped>

</style>
