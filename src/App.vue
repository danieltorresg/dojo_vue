<template>
   <v-app>
    <Toolbar />
    <v-main>
       <Search v-on:searchResult="searchResult" />
      <ImageList v-bind:items="items" />
    </v-main>
  </v-app>
</template>

<script>

import Toolbar from "./components/Toolbar";
import Search from "./components/Search";
import ImageList from "./components/ImageList";



export default {
  name: 'App',

  components: {
    Toolbar,
    Search,
    ImageList,
  },
  methods: {    
       searchResult(response){
         this.itmes = response;
         console.log(this.itmes);

       }

  },

  data: () => ({
    items: []
    //
  }),
};
</script>
