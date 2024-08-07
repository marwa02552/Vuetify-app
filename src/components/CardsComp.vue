<template>
   <v-card>
      <v-img src="../assets/work.png" ></v-img>
      <v-card-title>{{titl}}</v-card-title>
      <v-card-text>{{text}}</v-card-text>
      <v-divider></v-divider>
     <v-sheet class="rat">
      <v-card-actions>
         <v-btn>view details</v-btn>
         </v-card-actions>
          <v-rating half-increments color="#d9c036" v-model="rating"></v-rating>
     </v-sheet>
   </v-card>
     
</template>

<script>
export default {
   props:{
     titl:null,
     text:null,
     linke:null
},
   data() {
      return {
         rating:3.5
      }
   },
}
</script>

<style>
.rat{
   display: flex;
}
</style>