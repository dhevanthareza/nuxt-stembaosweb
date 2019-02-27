<template>
  <v-app>
    <v-toolbar absolute color="transparent" flat dark>
      <v-toolbar-title>Stemba OS</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn flat>About</v-btn>
        <v-btn flat>Features</v-btn>
        <v-btn flat>Download</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <div class="header">
      <v-layout class="header" row wrap justify-center align-center align-content-center>
        <v-flex xs12 style="text-align:center">
          <span class="judul1" style="color: white">Stemba OS</span>
          <br>
          <img class="wow bounceIn" width="600px" src="@/assets/img/stembaos.PNG">
        </v-flex>
      </v-layout>
    </div>
    <div id="about">
      <v-container>
        <v-layout row wrap align-center="">
          <v-flex xs12 sm6 style="text-align:center">
            <span class="gede">3.0</span>
            <br>
            <span class="judul1">Stemba OS</span>
          </v-flex>
          <v-flex xs12 sm6>
            <span class="description">an OS from developer to developer, with a built-in application that is very useful for developers and IT students, not only developers, a network engineer is suitable to use this, maybe you ask, why not like the previous version that has all applications for all majors in school, This version is only suitable for users in the IT field, because we realize Linux cannot be used by all fields of work, especially in the graphics field</span>
          </v-flex>
        </v-layout>
      </v-container>
    </div>
    <div id="download">
      <v-container>
      <v-layout row justify-center="">
        <v-flex xs6 style="text-align: center">
          <v-btn round outline color="white">Download Stemba OS 3.0</v-btn>
        </v-flex>
      </v-layout></v-container>
    </div>
  </v-app>
</template>

<script>
export default {
  head(){
    return{
      script: [
        {src: '/js/wow.js'},
        {src: '/js/my.js'}
      ],
      link: [
        { rel: 'stylesheet', href: '/css/animate.css' }
      ]
    }
  },
};
</script>
