<template>
   <v-container class="lending">
    <v-row>
        <v-col class="text" lg="6">
            <h2>welcom to vuetify app</h2>
             <p>
              Vuetify is a no design skills required UI Framework with beautifully handcrafted Vue Components
               Vuetify is a no design skills required UI Framework with beautifully handcrafted Vue Components</p> 
             <v-btn color="#62fc66">get started</v-btn>
        </v-col>
        <v-col lg="6">
           <v-img height="400" src="../assets/work.png"></v-img>
        </v-col>
    </v-row>
   </v-container>
</template>

<script>
export default {
    name:'LendingComp'
}
</script>


<style>
.lending{
    padding-top:200px ;
}
.v-container .text h2{
   text-transform: capitalize;
   font-size: 35px;
   font-weight: 600;
   color:  #151839;
   margin-bottom: 30px;
}
.v-container .text p{
    margin-bottom: 20px;
    font-size: 16px;
    color: #444551;
}
</style>