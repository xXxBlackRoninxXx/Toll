<template>
  <conteiner color="red">
    <div class="Search" >
      <input type="text" class="Search_input" v-model="query">
      <v-btn class="Search_button">Найти</v-btn>
    </div>
  </conteiner>
</template>

<script>
    export default {
        data(){
          return{
            query:''
          }
        }
    }
</script>

<style scoped>

</style>
