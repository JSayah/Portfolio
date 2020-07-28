<template>
  <v-app id='backColor'>
    <v-app-bar
      app
      id='gradient'
    >
      <div id='logoTop'><i class="fas fa-code"></i></div>
      <div class="d-flex align-center">
        <h1>Sayah.ME</h1>
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="./assets/Resume.txt"
        download
        text
      >
        <span class="mr-2">Download Resume</span>
        <i class="far fa-file"></i>
      </v-btn>
    </v-app-bar>

    <v-main>
      <HelloWorld/>
    </v-main>
    <Contact/>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import Contact from './components/Contact.vue'
export default {
  name: 'App',

  components: {
    HelloWorld,
    Contact,
  },

  data: () => ({
    //
  }),
};
</script>
<style>
#gradient{
  background: linear-gradient(90deg, rgba(142,0,137,1) 0%, rgba(119,9,121,1) 35%, rgba(0,212,255,1) 100%);
}
#backColor{
  background: black;
}
#logoTop{
  font-size: 150%;
  padding-right: 10px;
}
</style>
