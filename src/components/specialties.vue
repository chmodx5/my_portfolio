<template>
    <v-container>
        <v-layout row wrap class="grey--text text--darken-3"> 
            <v-flex xs12 class="text-xs-center pt-5">
                <h1 class="display-2 font-weight-light mb-2 text--darken-3 text--darken-4 grey--text">We specialize in</h1>
                <h4 class="subheading ">Specialized in Web Design, Android apps and Desktop apps</h4>
            </v-flex>
            <v-flex xs12 class="py-5">
                <v-layout>
                    <v-flex xs3 v-for="(specialtie, index) in specialties" :key="index" class="px-4">
                        <div>
                            <v-icon x-large color=" text--darken-4 grey--text"> {{specialtie.icon}} </v-icon>
                        </div>
                        <h4 class="headline text--darken-4 grey--text text-capitalize"> {{specialtie.title}} </h4>
                        <p style="text-align: justify;"> {{specialtie.content}} </p>
                    </v-flex>
                    
                </v-layout>
            </v-flex>
        </v-layout>
        
    </v-container>
</template>
<script>
export default {
  name: 'Specialties',
  data () {
    return {
        specialties: [
                { icon: 'fas fa-clipboard-list', title: 'content creation', content:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Provident temporibus magnam vel maxime iure voluptates odio, modi veniam dicta consequatur, natus nobis. Nostrum, mollitia. Maiores nulla earum eius illo nemo?' },
                { icon: 'fas fa-laptop', title: 'Web development', content:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Provident temporibus magnam vel maxime iure voluptates odio, modi veniam dicta consequatur, natus nobis. Nostrum, mollitia. Maiores nulla earum eius illo nemo?' },
                { icon: 'fas fa-tablet-alt', title: 'Android Apps', content:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Provident temporibus magnam vel maxime iure voluptates odio, modi veniam dicta consequatur, natus nobis. Nostrum, mollitia. Maiores nulla earum eius illo nemo?' },
                { icon: 'fas fa-desktop', title: 'Desktop Apps', content:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Provident temporibus magnam vel maxime iure voluptates odio, modi veniam dicta consequatur, natus nobis. Nostrum, mollitia. Maiores nulla earum eius illo nemo?' },
            ],
          
    }
  }
}
</script>
