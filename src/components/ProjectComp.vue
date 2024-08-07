<template>
    <v-container>
       <TextCiomp :titel="titel" :descrip="pr"/>
     <v-row>
        <v-col cols="4" v-for="item in tab" :key="item">
            <CardsComp :text="item.text2" :titl=" item.text"  />
        </v-col>
     </v-row>
    </v-container>
</template>

<script>
import TextCiomp from './TextCiomp.vue';
import CardsComp from './CardsComp.vue';
export default {
    name:'ProjectComp',
    components:{
        TextCiomp,
        CardsComp
    },
    data() {
        return {
            titel:'project',
            pr:'Vuetify is a no design skills required UI Framework with beautifully handcrafted Vue Components',
            
            tab:[
               {
                text:'web site devellopement',
                text2:'Vuetify is a no design skills required UI Framework with beautifully handcrafted Vue Components.',
                links:'work.png'
               },
               {
                text:'desktop devellopemnt',
                text2:'Vuetify is a no design skills required UI Framework with beautifully handcrafted Vue Components.',
                links:'about.png'
            },
               {
                text:'mobile devellopemnt',
                text2:'Vuetify is a no design skills required UI Framework with beautifully handcrafted Vue Components.',
                links:'logo.jpg'
               }
            ]
        }
        
    },
}
</script>