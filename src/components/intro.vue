<template>
  <v-parallax
    dark
    src=" https://source.unsplash.com/x1QSu6XexIw"
  >
    <v-layout column justify-center>
      <div class="mx-9 pa-3 " style="background-color: rgb(32,29,40,0.6); border-radius: 5px;"> 
        <h1 class="display-3 font-weight-light  mb-2 text-capitalize">Hello</h1>
        <h1 class="display-2 font-weight-light mb-2 text-capitalize">We are a <span class="yellow--text text--darken-2">software design</span>  company</h1>
        <h4 class="headline font-weight-thin text-capitalize">Specialized in Web Design, Android apps and Desktop apps</h4>
        <v-btn to="/about" class="ml-0 yellow darken-2 white--text text-capitalize font-weight-light title" round> 
          About us
        </v-btn>
      </div>
    </v-layout>
  </v-parallax>
</template>

<script>
  export default {
    name:'intro',
    data: () => ({
    
    })
  }
</script>

<style>

</style>
