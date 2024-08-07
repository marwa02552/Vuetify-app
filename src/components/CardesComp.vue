<template>
    <v-container class="cards">
        <v-card>
         <v-img gradient="to bottom, rgba(0,0,0,0.5),rgba(0,0,0,0.3)" height="300" :src="require(`../assets/${link}`)"><h3>{{text}}</h3></v-img> 
        </v-card>
    </v-container>
</template>

<script>
export default {
    props:{
      link:null,
      text:null
    },
   
}
</script>

<style>
.cards .v-card{
  position: relative;
}
.cards h3{
    position: absolute;
    bottom: 20px;
    color: #151839;
    text-transform: capitalize;
    font-size: 18px;
    left: 10px;
}
</style>