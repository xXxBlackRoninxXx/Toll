<template>
  <v-container>
    <v-alert  :value="alert" color="blue" type="warning">
      Действующий Email и пароль
    </v-alert>
  <v-form @submit.prevent="submit">

    <v-text-field
      v-model="email"
      label="E-mail"
      required
    ></v-text-field>

    <v-text-field
      v-model="password"
      :rules="password"
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
            password:null,
            alert:false,
          }
        },
      methods:{
          submit(){
            if(!this.email && !this.password){
              this.alert=true
            }
            console.log(`Email is ${this.email} and Password is ${this.password}`)
          }
      }
    }
</script>

<style scoped>

</style>
