<template>
  <v-container>
    <v-card width="400px"   variant="outlined" prepend-icon="mdi-home" title="card1" subtitle="welcom to card1" text="this i sykdbc lJXuzbe ndhcouha sjdncoauehnçfuabe^fcnapeivbaeibviabevibaervbib">
      <v-card-action>
        <v-btn>clique me1</v-btn>
         <v-btn>clique me2</v-btn>
         <v-icon>mdi-heart</v-icon>
      </v-card-action>
    </v-card>

    <v-card  width="600px">
      <v-card-text>
        <p >welcom</p>
        <h1>this is titele card</h1>
        <p>this i sykdbc lJXuzbe ndhcouha sjdncoauehnçfuabe^fcnapeivbaeibviabevibaervbib</p>
      </v-card-text>
      <v-card-action>
        <v-btn @click="change=true">learn more</v-btn>
      </v-card-action>
      <v-expand-transition>
        <v-card v-if="change"  class="transition-fast-in-fast-out v-card--reveal">
          <v-card-text class="pb-0">
          <p class="text-h4 text--primary">
            Origin
          </p>
          <p>late 16th century (as a noun denoting a place where alms were distributed): from medieval Latin eleemosynarius, from late Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’ </p>
        </v-card-text>
        <v-action>
          <v-btn @click="change=false">close</v-btn>
        </v-action>
        </v-card>
      </v-expand-transition>
    </v-card>


    <v-card width="600px">
       <v-img src="../assets/muffin.jpg" cover height="250"> <v-card-title >Top 10 Australian beaches</v-card-title></v-img>
       <v-card-item>
        <v-card-title>Cafe Badilico</v-card-title>
         <v-card-subtitel>frr for this 3 days</v-card-subtitel>
       </v-card-item>
       <v-card-text>
        <v-row   align="center" class="mx-6">
          <v-rating
          :model-value="3.5"
          color="amber"
          density="compact"
          half-increments
          size="small"
        ></v-rating>
        <div class="text-red mx-2"> 4.230 (12.33)</div>
        </v-row>
        <div class="my-5">$ italin,cafe</div>
        <div>Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
       </v-card-text>
       <v-divider></v-divider>

       <div class="mx-5 my-4">Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
    
       <v-card-title >Tonight's availability</v-card-title>
     <v-row align="center" class="mx-6 my-3">
      <v-chip class="mx-2">12.33 pm</v-chip>
      <v-chip class="mx-2">15..36 pm</v-chip>
      <v-chip class="mx-2">5.55 pm</v-chip>
      <v-chip class="mx-2">9.28 pm</v-chip>
     </v-row>
     <v-card-action>
      <v-btn class="mx-4 my-4 " color="deep-purple-lighten-2">reserved</v-btn>
     </v-card-action>
      </v-card>


      <v-card width="300" class="mx-5">
        <v-img src="../assets/muffin.jpg" cover height="250">
          <v-icon>mdi-home</v-icon>
          <v-icon>mdi-heart</v-icon>
        </v-img>
        <v-card-title>Cafe Badilico</v-card-title>
        <v-card-subtitle>
      1,000 miles of wonder
    </v-card-subtitle>
        <v-card-action><v-btn @click="showtext">explore</v-btn></v-card-action>
        <v-expend-transition>
          <v-card v-show="show">
            <v-card-title>Cafe Badilico</v-card-title>
            <v-card-text>
          I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape.
        </v-card-text>

          </v-card>
        </v-expend-transition>
      </v-card>
  </v-container>
</template>

<script>
export default {
  name:'NavComp',
  data() {
    return {
      change:false,
      show:false
    }
  },
  methods: {
    showtext(){
      this.show=!this.show
    }
  },
}
</script>

<style>
.v-container{
  padding-left: 2%;
  padding-right: 2%;
  }
</style>