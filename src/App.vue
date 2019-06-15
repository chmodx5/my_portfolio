<template>
  <v-app light>
    <v-toolbar app height="60" color='rgb(255,255,255,0.9)' flat>
      <v-toolbar-title class="headline text-uppercase">
        <span>Portfolio </span>
        <span class="font-weight-light yellow--text text--darken-2"> Me</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-menu offset-y auto close-delay="2" min-width="200px">
      <template v-slot:activator="{ on }">
        <v-btn color="yellow darken-2" icon large dark v-on="on" flat>
          <v-icon>fas fa-stream</v-icon>
        </v-btn>
      </template>
      <v-list>
        <div v-for="(item,index) in items" :key="index">
          <v-list-tile :to="item.link">
            <v-list-tile-title>{{ item.title }}</v-list-tile-title>
          </v-list-tile>
        </div>
      </v-list>
    </v-menu>
    </v-toolbar>

    <v-content>
      <router-view/>
    </v-content>
  </v-app>
</template>

<script>

export default {
  name: 'App',
  data () {
    return {
        items: [
                  { title: 'Home', link: '/' },
                  { title: 'About', link: '/about'},
                ],
          
    }
  }
}
</script>
