<template>
  <div id="app">
    
    <desafioVue
        :listado="listado_uno"
        :estilo="estilo_uno"
        :clase="clase_uno"
        ></desafioVue>
        
        <desafioVue
        :listado="listado_dos"
        :estilo="estilo_dos"
        :clase="clase_dos"
        ></desafioVue>

        <desafioVue
        :listado="listado_tres"
        :estilo="estilo_tres"
        :clase="clase_tres"
        ></desafioVue>

  </div>
</template>

<script>

/* eslint-disable */

import HelloWorld from './components/HelloWorld.vue'
import desafioVue from './components/desafioVue.vue'


export default {
  name: 'App',
  components: {
    HelloWorld,
    desafioVue
  },
  data(){
    return{
      
                listado_uno: [{"id":1,"nombre":"Renault"},
                {"id":2,"nombre":"Chevrolet"},
                {"id":3,"nombre":"Peugeot"},
                {"id":4,"nombre":"Mercedes Benz"}],
                listado_dos: [{"id":1,"nombre":"Helado"},
                {"id":2,"nombre":"Carne"},
                {"id":3,"nombre":"Pastas"},
                {"id":4,"nombre":"Brownie"}],
                listado_tres: [{"id":1,"nombre":"Futbol"},
                {"id":2,"nombre":"Basquet"},
                {"id":3,"nombre":"Tenis"},
                {"id":4,"nombre":"Natacion"}],
                estilo_uno: { 'background': '#F7FF00'},
                estilo_dos: { 'background': '#56220E'},
                estilo_tres: { 'background': '#00A2FF'},
                clase_uno: { 'letra-azul': true},
                clase_dos: { 'letra-amarilla': true},
                clase_tres: { 'letra-azuloscuro': true},
                flag: false
            }
    }
  }


</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.letra-azul { 
            color: rgb(8, 0, 255);
        }
        .letra-amarilla { 
            color: rgb(255, 217, 0);
        }
        .letra-azuloscuro { 
            color: rgb(0, 7, 59);
        }

        /*Estilo general de tabla*/
        table {
            font-family: arial, sans-serif;
            border-collapse: collapse;
            width: 100%;
          }
          
          td, th {
            border: 1px solid #dddddd;
            text-align: left;
            padding: 8px;
          }
</style>
