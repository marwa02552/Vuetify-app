<template>
    <v-container>
       <TextCiomp :titel="titel" :descrip="text"/>
       <v-row >
        <v-col align="center" class="btn1" >
            <v-chip  v-for="ti in tab2" :key="ti" class="mx-2"  color="green"  text-color="white">{{ti}}</v-chip>
        </v-col>
       </v-row>
      <v-row >
        <v-col v-for="links , i in tab" :key="i" cols="3">
         <CardesComp :link="links" :text="tab1[i]"/>
        </v-col>
      </v-row>
    </v-container>
</template>

<script>
import TextCiomp from './TextCiomp.vue';
import CardesComp from './CardesComp.vue';
export default {
    name:'PortfoComp',
    components:{
        TextCiomp,
        CardesComp
    },
    data() {
        return {
            titel:'portfolio',
            text:' Vuetify is a no design skills required UI Framework with beautifully handcrafted Vue Components',
            tab:['about.png','work.png','logo.png','logo.svg'],
            tab1:['desktop app1','desktop app2','desktop app3','desktop app4'],
            tab2:['web site','mobile app','desktop app']
        }
    },
}
</script>

<style>
.test{
    text-align: center;
}
.btn1 .v-chip {
  text-transform: capitalize;
}
</style>