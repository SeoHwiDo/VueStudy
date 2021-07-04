<template>
  <v-app>
    <v-content>
      <toolbar></toolbar>
      <home></home>
      <homebutton></homebutton>
    </v-content>
  </v-app>  
</template>

<script>
import Home from './components/Home';
import Homebutton from './components/Homebutton';
import Toolbar from './components/Toolbar'
export default {
  name: 'App',

  components: {
    Homebutton,Home,Toolbar,
  },
};
</script>
