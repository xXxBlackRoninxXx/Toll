<template>
    <div class="Search">
      <input type="text" class="Search_input" v-model="query">
      <v-btn class="Search_button">Найти</v-btn>
    </div>
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
