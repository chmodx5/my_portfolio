<template>
    <v-container>
        <v-layout row wrap>
            <v-flex xs12 class="text-xs-center pt-5">
                <h1 class="display-2 font-weight-light mb-2 ">Our Working proces</h1>
                <h4 class="subheading">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nihil quos tenetur sapiente magnam, nesciunt numquam obcaecati</h4>
            </v-flex>
            <v-flex xs12 class="py-5">
                <v-layout>
                    <v-flex xs3 v-for="(workprocess, index) in working_process" :key="index" class="px-4">
                        <div>
                            <v-badge color="cyan" right overlap>
                                <template v-slot:badge>
                                    <span>{{workprocess.process_num}}</span>
                                </template>
                                    <v-icon x-large> {{workprocess.icon}} </v-icon>
                            </v-badge>
                            
                        </div>
                        <h4 class="headline"> {{workprocess.title}} </h4>
                        <p style="text-align: justify;"> {{workprocess.content}} </p>
                    </v-flex>
                    
                </v-layout>
            </v-flex>
        </v-layout>
        
    </v-container>
</template>
<script>
export default {
  name: 'workingProcess',
  data () {
    return {
        working_process: [
                {process_num: 1, icon: 'fas fa-arrow-circle-right', title: 'content creation', content:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Provident temporibus magnam vel maxime iure voluptates odio, modi veniam dicta consequatur, natus nobis. Nostrum, mollitia. Maiores nulla earum eius illo nemo?' },
                {process_num: 2, icon: 'fas fa-arrow-circle-right', title: 'Web development', content:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Provident temporibus magnam vel maxime iure voluptates odio, modi veniam dicta consequatur, natus nobis. Nostrum, mollitia. Maiores nulla earum eius illo nemo?' },
                {process_num: 3, icon: 'fas fa-arrow-circle-right', title: 'Android Apps', content:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Provident temporibus magnam vel maxime iure voluptates odio, modi veniam dicta consequatur, natus nobis. Nostrum, mollitia. Maiores nulla earum eius illo nemo?' },
                {process_num: 4, icon: 'fas fa-arrow-circle-right', title: 'Desktop Apps', content:'Lorem ipsum dolor sit amet consectetur, adipisicing elit. Provident temporibus magnam vel maxime iure voluptates odio, modi veniam dicta consequatur, natus nobis. Nostrum, mollitia. Maiores nulla earum eius illo nemo?' },
            ],
          
    }
  }
}
</script>
