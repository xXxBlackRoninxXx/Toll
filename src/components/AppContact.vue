<template>
  <v-layout mt-3>
    <v-flex xs12 sm8 offset-sm2>
      <v-card class="elevation-24">
        <v-img
          src="https://scontent-lga3-1.cdninstagram.com/vp/c57e58848fad563dec1e1d9f71c9fcd7/5C58C4C4/t51.2885-15/sh0.08/e35/s750x750/38920088_306859846742967_6514810998224846848_n.jpg?ig_cache_key=MTg0NTYwODU2MDA0ODUxNTczMg%3D%3D.2"
          aspect-ratio="2.75"
        ></v-img>

        <v-card-text primary-title>
          <div>
            <h3 class="headline mb-3" >Рубцовский институт (филиал) АлтГУ</h3>
            <v-avatar
              size="80"
              color="grey lighten-4"
            >
              <img src="https://rb.asu.ru/public/design/images/logotype/logoRI-2017.png">
            </v-avatar>
            <div class="text-md-center"> Адрес: 	658225, г. Рубцовск, пр. Ленина 200-б <br> Телефон:	(8-385-57) 4-20-04</div>
          </div>
        </v-card-text>

        <v-card-actions>
          <v-btn flat color="blue darken-4">Поделиться</v-btn>
          <v-btn flat color="blue darken-4">Изучить</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
    export default {
        name: "AppContact"
    }
</script>

<style scoped>

</style>
