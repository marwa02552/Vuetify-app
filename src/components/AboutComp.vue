<template>
    <v-container>
     <v-row>
        <v-col lg="6">
            <v-img src="../assets/about.png"></v-img>
        </v-col>
        <v-col lg="6" class="text">
            <h4>about us</h4>
            <p>Vuetify is a no design skills required UI Framework with beautifully handcrafted Vue Components</p>
            <v-list class="listbtn"  >
                <v-list-item ><v-icon color="#62fc66" class="icon">mdi-check-all</v-icon> Vuetify is a no design skills required</v-list-item>
                <v-list-item > <v-icon color="#62fc66" class="icon">mdi-check-all</v-icon>Vuetify is a no design skills required</v-list-item>
                <v-list-item ><v-icon color="#62fc66" class="icon">mdi-check-all</v-icon>Vuetify is a no design skills required</v-list-item>
            </v-list>
            <p>uetify is a no design skills required UI Framework with beautifully handcrafted Vue Componentsuetify is a no design skills required UI Framework with beautifully handcrafted Vue Components</p>
        </v-col>
     </v-row>
    </v-container>
</template>

<script>
export default {
    name:'AboutComp'
}
</script>
<style>
.v-container .text{
    margin-top: 60px;
}
.v-container .text h4{
    text-transform: uppercase;
    font-size: 35px;
    color: #151839;
    margin-bottom: 10px;
}
.v-container .text p{
    font-size: 18px;
    color: #444551;
    margin-bottom: 10px;
}
.v-container .listbtn .icon{
   margin-right: 10px;
}
.v-container .listbtn{
    margin-bottom: 10px;
}
</style>