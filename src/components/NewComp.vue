<template>
    <div>
       <v-hover close-delay="2000"  open-delay="2000" v-slot="{ isHovering, props }">
        
        <v-card   v-bind="props"   title="hover on me" text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate "  >   
            <v-expand-transition>
          <div
            v-if="isHovering"
            class="d-flex transition-fast-in-fast-out bg-orange-darken-2 v-card--reveal text-h2"
            style="height: 100%;"
          >
            $14.99
          </div>
        </v-expand-transition>
        </v-card>
       </v-hover>

       <v-card   class="hover" title="hover on me" text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate " >   
        </v-card>


       <v-btn @click="show=true">show the messege</v-btn>
        <v-snackbar  :timeout="2000"   color="blue-grey"    elevation="24" multi-line v-model="show"> hello welcom to our web site <v-btn @click="show=false"  variant="link">close</v-btn></v-snackbar>
    
      <v-list>
        <v-list-item prepend-icon="mdi-home" title="home"></v-list-item>
        <v-list-group >
            <template v-slot:activator="{ props }">
          <v-list-item
            v-bind="props"
            prepend-icon="mdi-account-circle"
            title="Users"
          ></v-list-item>
        </template>
        <v-list-item>item one</v-list-item>
        <v-list-item>item one</v-list-item>
        <v-list-item>item one</v-list-item>
       <v-list-group>
         <template v-slot:activator="{props}">
            <v-list-item v-bind="props" title="action" ></v-list-item>
         </template>
         <v-list-item>item 1 of action</v-list-item> 
         <v-list-item>item 1 of action</v-list-item> 
         <v-list-item>item 1 of action</v-list-item> 
       </v-list-group>
        </v-list-group>
      </v-list>
   
   </div>
</template>

<script>
export default {
  name:'NewCopm',
  data() {
    return {
        show:false,
        items: [
        {
          title: 'Item #1',
          value: 1,
        },
        {
          title: 'Item #2',
          value: 2,
        },
        {
          title: 'Item #3',
          value: 3,
        },
      ],
    }
    }
  }
</script>

<style>
.hover{
    background-color: pink;
    padding: 50px;
}
</style>