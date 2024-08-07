<template>
  <div>
    <v-expansion-panels   v-model="panel"   multiple  :readonly="false" >
      <v-expansion-panel title="panele1" value="panel2" text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate minima"></v-expansion-panel>
      <v-expansion-panel     expand-icon="mdi-menu-down" title="panele2" value="panele" text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate minima"></v-expansion-panel>
      
    </v-expansion-panels>

    <v-row no-gutters>
      <v-col
        v-for="n in 3"
        :key="n"
        cols="12"
        sm="4"
      >
        <v-sheet class="ma-2 pa-2">
          One of three columns
        </v-sheet>
      </v-col>
    </v-row>
    
  
   <v-row  no-gutters>
    <v-col 
        offset="4" cols="4">welcom </v-col>
    <v-col>welcom</v-col>
    <v-col 
        offset="4">welcom</v-col>
   </v-row>

   <v-row  no-gutters>
    <v-col cols="3" v-for="n in 12" :key="n">one</v-col>
   </v-row>
    <div>{{panel}}</div>
  </div>

  <v-row>
    <v-col cols="3" offset="3">this is withe poffset3</v-col>
    <v-col
        cols="4"
        offset="4"
      >
        <v-sheet >
          .v-col-4 .offset-4
        </v-sheet>
      </v-col>
  </v-row>
</template>

<script>
export default {
  name:'HelloWorld',
  data() {
    return {
      panel:[],
    
      disabled:false
    }
  },
}
</script>