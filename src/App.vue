<template>
  <v-app>
    <v-content>
      <!-- <home></home> -->
      <homebutton></homebutton>
    </v-content>
  </v-app>  
</template>

<script>
import Home from './components/Home';
import homebutton from './components/Homebutton';

export default {
  name: 'App',

  components: {
    Home,homebutton,
  },
};
</script>
