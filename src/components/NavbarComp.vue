<template>
  
    <v-container>
        <v-app-bar>
        <v-app-bar-title>vuetifyProject</v-app-bar-title>
       <v-btn >
        <v-icon  @click="affiche" v-show="menu">mdi-format-list-bulleted</v-icon>
       </v-btn>
        <v-spacer></v-spacer>
        <v-list class="liste" v-for="item in menus" :key="item" v-show="!menu">
            <v-list-item link>{{item}}</v-list-item>
        </v-list>
        <v-spacer></v-spacer>
        <v-list class="icon" v-show="!menu">
            <v-list-item><v-btn>get started</v-btn></v-list-item>
        </v-list>
      </v-app-bar>
  
    </v-container>
</template>

<script>
export default {
    name:'NavbarComp',
    data() {
        return {
            menus:[
                'home','aboute us','portfolio','project','gallery','contact'
            ],
            item:null,
            windowwidth:null,
            list:null,
            menu:null
        }
    },
    created() {
        window.addEventListener('resize',this.checksize)
        this.checksize
    },
    methods: {
       checksize(){
        this.windowwidth=window.innerWidth
        if(this.windowwidth<800){
          this.menu=true
          this.list=true
          return
        }else{
            this.menu=false
            this.list=false
            return
        }
       }
    },
    affiche(){
        this.list=!this.list
        console.log("i m work")
    }
}
</script>

<style>
.v-app-bar{
    padding-left:6%;
    padding-right:6%;
}

.icon .v-list-item .v-btn{
    color: #62fc66;
    border: #151839 solid 1px;
}
.liste{
    display: flex;
}
.liste .v-list-item{
    text-transform: capitalize;
    color:  #151839;
    
}
.v-app-bar-title{
   text-transform: capitalize;
   font-size: 25px;
   color:  #62fc66;
   font-weight: 600;
}
.phone{
    display: flex;
    flex-direction: column;
    position: absolute;
    top: 50px;
}
</style>