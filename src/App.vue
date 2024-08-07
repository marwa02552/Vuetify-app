<template>
 <v-app>
  <NavbarComp/>
   <LendingComp/>
   <AboutComp/>
   <PortfoComp/>
   <ProjectComp/>
 </v-app>
</template>

<script>

import NavbarComp from './components/NavbarComp.vue';
import LendingComp from './components/LendingComp.vue';
import AboutComp from './components/AboutComp.vue';
import PortfoComp from './components/PortfoComp.vue';
import ProjectComp from './components/ProjectComp.vue';
export default {
  name: 'App',
  components:{
    NavbarComp,
    LendingComp,
    AboutComp,
    PortfoComp,
    ProjectComp
    
  }
}
</script>

<style>
*{
box-sizing: border-box;
padding: 0;
margin: 0;
}
:root{
 --mainPadding:9%;
}
</style>

