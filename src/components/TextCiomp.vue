<template>
    <v-container class="header">
        <h1>{{titel}}</h1>
        <p>{{descrip}}</p>
    </v-container>
</template>

<script>
export default {
   props:{
    titel:null,
    descrip:null
   }
}
</script>

<style>
.header{
    margin-top: 40px;
    margin-bottom: 40px;
    text-align: center;
}

.header h1{
    color:#62fc66;
    font-size: 35px;
    margin-bottom: 10px;
    text-transform: capitalize;
}
.header p{
    font-size: 18px;
    color: #444551;
}
</style>