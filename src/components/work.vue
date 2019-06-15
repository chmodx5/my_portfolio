<template>
<v-container>
  <div>
   <v-layout row wrap>
    <v-flex xs12 class="text-xs-center py-5">
        <h1 class="display-2 font-weight-light mb-2 text--darken-3 text--darken-4 grey--text">We specialize in</h1>
        <h4 class="subheading ">Specialized in Web Design, Android apps and Desktop apps</h4>
    </v-flex>
    <v-flex v-for="(items, index) in gallery" :key="index" xs6 md4 lg3 class="px-4 mb-4">
      <v-card  color="">
        <v-img :src="items.image" aspect-ratio="1.5" >
        </v-img>

        <v-card-title primary-title class="mt-0 pt-2 pb-2 ">
          <div to="http://www.google.com">
            <div class="title font-weight-regular mt-0">   {{items.title}}     </div>
            <span class="grey--text">  {{items.subtitle}}   </span>
            <v-btn outline round color="yellow darken-3" class="mx-0"> visit </v-btn>
          </div>
        </v-card-title>
      </v-card>
    </v-flex>
  </v-layout>
  
  </div>
  </v-container>
</template>
<script>
export default {
    name:'work',
    data () {
      return {
          show: false,
          gallery:[
              {image: 'https://cdn.vuetifyjs.com/images/cards/sunshine.jpg', title: 'www.website.com',  subtitle: '1,000 miles of wonder', readMore: "I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape."},
              {image: 'https://cdn.vuetifyjs.com/images/cards/sunshine.jpg', title: 'www.website.com',  subtitle: '1,000 miles of wonder', readMore: "I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape."},
              {image: 'https://cdn.vuetifyjs.com/images/cards/sunshine.jpg', title: 'www.website.com',  subtitle: '1,000 miles of wonder', readMore: "I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape."},
              {image: 'https://cdn.vuetifyjs.com/images/cards/sunshine.jpg', title: 'www.website.com',  subtitle: '1,000 miles of wonder', readMore: "I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape."},
              {image: 'https://cdn.vuetifyjs.com/images/cards/sunshine.jpg', title: 'www.website.com',  subtitle: '1,000 miles of wonder', readMore: "I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape."},
              {image: 'https://cdn.vuetifyjs.com/images/cards/sunshine.jpg', title: 'www.website.com',  subtitle: '1,000 miles of wonder', readMore: "I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape."},
              {image: 'https://cdn.vuetifyjs.com/images/cards/sunshine.jpg', title: 'www.website.com',  subtitle: '1,000 miles of wonder', readMore: "I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape."},
              {image: 'https://cdn.vuetifyjs.com/images/cards/sunshine.jpg', title: 'www.website.com',  subtitle: '1,000 miles of wonder', readMore: "I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape."},
          ]
      }
    },
    methods: {
     
    }
  }
</script>

