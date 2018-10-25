<template>
  <container>
  <v-carousel >
    <v-carousel-item height="700"
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>

      <div>
      <router-view name="about"/>

      </div>

  </container>



</template>


<script>
  export default {
    data () {
      return {

        items: [
          {
            src: 'http://snim.net/wp-content/uploads/2016/03/%D0%B5%D0%BD%D0%BE%D1%82-%D1%81-%D0%B4%D0%B5%D1%82%D1%91%D0%BD%D1%8B%D1%88%D0%B5%D0%BC-%D0%B8%D0%B4%D1%83%D1%82-%D0%BF%D0%BE-%D0%B2%D0%BE%D0%B4%D0%B5.jpg'
          },
          {
            src: 'http://www.gandex.ru/upl/oboi/gandex.ru-17782_8867_hanginout_2560x1600.jpg'
          },
          {
            src: 'http://snim.net/wp-content/uploads/2016/04/%D0%B5%D0%BD%D0%BE%D1%82.jpg'
          },
        ]
      }
    }
  }
</script>

<style>

</style>
