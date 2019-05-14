<template>
  <v-app>
    <v-toolbar absolute color="transparent" flat dark>
      <v-toolbar-title>Stemba OS</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn @click="$vuetify.goTo(about, options)" flat>About</v-btn>
        <v-btn flat>Features</v-btn>
        <v-btn @click="$vuetify.goTo(download, options)" flat>Download</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <div id="header" class="header">
      <v-layout class="header" row wrap justify-center align-center align-content-center>
        <v-flex xs12 style="text-align:center">
          <span class="judul1" style="color: white">Stemba OS</span>
          <br>
          <img class="laptop wow bounceIn" src="@/assets/img/stembaos.PNG">
        </v-flex>
      </v-layout>
    </div>
    <div id="about">
      <v-container style="background-color: white">
        <v-layout row wrap align-center>
          <v-flex class="wow fadeInLeft" sm12 md6 style="text-align:center">
            <span class="gede">3.0</span>
            <br>
            <span class="judul1">Stemba OS</span>
          </v-flex>
          <v-flex class="wow fadeInRight" sm12 md6>
            <span
              class="description"
            >an OS from developer for developer, with a built-in application that is very useful for developers and IT students, not only developers, a network engineer is suitable to use this, maybe you ask, why not like the previous version that has all applications for all majors in school, This version is only suitable for users in the IT field, because we realize Linux cannot be used by all fields of work, especially in the graphics field</span>
          </v-flex>
        </v-layout>
      </v-container>
    </div>
    <div id="feature">
      <v-container>
        <v-layout row wrap> 
          
        </v-layout>
      </v-container>
    </div>
    <div id="download" class="download">
      <v-layout row wrap justify-center align-center>
        <v-flex
          xs12
          sm12
          md6
          style="text-align: center;background-color: #0a4b83;padding: 30px 20px;border-top-left-radius: 25px;border-top-right-radius: 25px;"
        >
          <img width="80%" class="wow bounceIn" src="@/assets/img/stembaos.PNG">
        </v-flex>
        <v-flex xs12 sm12 md6 style="text-align: center;background-color: #084071;padding: 20px">
          <v-btn class="wow bounceIn" round outline color="white">Download Stemba OS 3.0</v-btn>
          <v-btn class="wow bounceIn" round outline color="white">Download Stemba OS 2.0</v-btn>
          <v-btn class="wow bounceIn" round outline color="white">Download Stemba OS 1.0</v-btn>
        </v-flex>
      </v-layout>
    </div>
  </v-app>
</template>

<script>
export default {
  head() {
    return {
      script: [{ src: "/js/wow.js" }, { src: "/js/my.js" }],
      link: [
        { rel: "stylesheet", href: "/css/animate.css" },
        { rel: "stylesheet", href: "/css/style.css" }
      ]
    };
  },
  computed: {
    header() {
      const value = "#header";
      if (!isNaN(value)) {
        return Number(value);
      } else {
        return value;
      }
    },
    about() {
      const value = "#about";
      if (!isNaN(value)) return Number(value);
      else return value;
    },
    tentang() {
      const value = "#tentang";
      if (!isNaN(value)) return Number(value);
      else return value;
    },
    download() {
      const value = "#download";
      if (!isNaN(value)) return Number(value);
      else return value;
    },
    options() {
      return {
        duration: 1000,
        offset: -60,
        easing: "easeInOutCubic"
      };
    }
  }
};
</script>
