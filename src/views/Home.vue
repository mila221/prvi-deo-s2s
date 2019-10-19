<template>
  <div>
     <v-parallax src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"> 
     <h1 class="text-center">GLavni naslov home stranica</h1>
     </v-parallax>

    <h1 class="text-center py-5">Lorem ipsum dolor sit.</h1>

     <v-row justify="center" align="center">


     
     <div class="box">
       <div class="circle">
         <v-icon class="icon">
           mdi-account
         </v-icon>
        
       </div>
       <h2 class="py-2">Lorem, ispum dolor.</h2>
       <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ea tempore in aut deleniti qui dignissimos at maiores numquam vel facilis, quasi saepe asperiores eaque earum corporis dolores! Voluptatum reprehenderit cumque iste porro expedita veritatis dolorum molestias dolor veniam. Iste laudantium facere voluptatem alias minus architecto eum dolorem adipisci dolor! Quasi!</p>
     </div>
     <div class="box">
       <div class="circle">
         <v-icon class="icon">
           mdi-account
         </v-icon>
        
       </div>
       <h2 class="py-2">Lorem, ispum dolor.</h2>
       <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ea tempore in aut deleniti qui dignissimos at maiores numquam vel facilis, quasi saepe asperiores eaque earum corporis dolores! Voluptatum reprehenderit cumque iste porro expedita veritatis dolorum molestias dolor veniam. Iste laudantium facere voluptatem alias minus architecto eum dolorem adipisci dolor! Quasi!</p>
     </div>
     <div class="box">
       <div class="circle">
         <v-icon class="icon">
           mdi-account
         </v-icon>
        
       </div>
       <h2 class="py-2">Lorem, ispum dolor.</h2>
       <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ea tempore in aut deleniti qui dignissimos at maiores numquam vel facilis, quasi saepe asperiores eaque earum corporis dolores! Voluptatum reprehenderit cumque iste porro expedita veritatis dolorum molestias dolor veniam. Iste laudantium facere voluptatem alias minus architecto eum dolorem adipisci dolor! Quasi!</p>
     </div>
     </v-row>


    <h1 justify="center" align="center">Cesta pitanja</h1>
    <v-row justify="center" align="center">
      <v-col cols="11" sm="7">
 <v-expansion-panels focusable>
       <v-expansion-panel>
         <v-expansion-panel-header>Item 1</v-expansion-panel-header>
         <v-expansion-panel-content>Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit commodi cum 
           incidunt iste exercitationem voluptates sit officia corrupti reprehenderit alias, nemo nostrum voluptatum
            at provident voluptas ipsum esse sapiente magni!</v-expansion-panel-content>
       </v-expansion-panel>

        <v-expansion-panel>
         <v-expansion-panel-header>Item 3</v-expansion-panel-header>
         <v-expansion-panel-content>Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit commodi cum 
           incidunt iste exercitationem voluptates sit officia corrupti reprehenderit alias, nemo nostrum voluptatum
            at provident voluptas ipsum esse sapiente magni!</v-expansion-panel-content>
       </v-expansion-panel>

        <v-expansion-panel>
         <v-expansion-panel-header>Item 2</v-expansion-panel-header>
         <v-expansion-panel-content>Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit commodi cum 
           incidunt iste exercitationem voluptates sit officia corrupti reprehenderit alias, nemo nostrum voluptatum
            at provident voluptas ipsum esse sapiente magni!</v-expansion-panel-content>
       </v-expansion-panel>

     </v-expansion-panels>

      </v-col>
    </v-row>

    
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',
  
}
</script>

<style scoped>
.box{
  width: 300px;
  padding: 20px;
  text-align: center;
  display: inline-block;
}
.circle{
  width: 150px;
  height: 150px;
  border-radius: 50%;
  border: 15px solid blue;
  display: inline-block;
}
.circle:hover{
  border-color: rgb(39, 199, 228);
}
.icon{
  font-size: 60px;
  position: relative;
  top: 50%;
  transform: translateY(-50%);
  
}
</style>
