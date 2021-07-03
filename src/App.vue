<template>
  <v-app>
    <v-content>
      <home></home>
    </v-content>
  </v-app>  
</template>

<script>
import Home from './components/Home';

export default {
  name: 'App',

  components: {
    Home,
  },
};
</script>
