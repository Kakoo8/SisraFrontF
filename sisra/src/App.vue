<template>

  <div id="app" >

  
    
    <div class="container">
      <h2 class="subtitle">
      <nav class="level">
                <p class="level-item">
                  <img src="http://en.usach.cl/sites/default/files/logo-usach_2.png" width="40" height="auto">
                  SISRA
                </p>
                <p class="level-item has-text-centered">
                  Nombre Alumno: <p v-show="valido">Claudio Urrutia<p>
                </p>
                <p class="level-item has-text-centered">
                  Carrera: <p v-show="valido">Ingenieria en Ejecución Informática<p>
                </p>
                <p class="level-item has-text-centered">
                  
                </p>
                <p class="level-item has-text-centered">
                  
                </p>
                <p class="level-item has-text-centered">
                <input class="input is-warning" type="text" v-on:keyup.enter="actualizar" placeholder="Ingrese Rut">
                  
                </p>
              </nav>
        
      
      </h2>

    </div>
 
       
      
      
  
    <div class="container is-fluid" id="container2">
      
        <div class="column " id="malla" v-show="valido">
          <Malla ></Malla>

        </div>
        <!--<div class="column">
          <Codigo/>
          <br>
          <Info/>
        </div> is-four-fifths-->
        
    </div>
      
    
  

     </div>
</template>

<style>

.section {
  display: flex;
  
  background-color: gray;
  padding: 1rem 1.1rem;
  
}

#container2{
  display: flex;
  width: -webkit-fill-available;
  
  min-height: 100%;
  max-height: 100%;
  background-color: transparent;
}
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    background-color: #ecf1c1; 
    height: 100%;

    background-position: center;
 
}
  html, body, #app {
    margin: 0;
    
    max-height:100%;
    min-height:100%;
    max-width: 100%;
    display:flex;
    flex-flow:column;
  }
 #malla{
   overflow:auto;

   
 } 



</style>
<script>

import Codigo from './components/CodigoColor';
import Info from './components/Info';
import Malla from './components/Malla';
export default {
  name: 'App',
  components: {
    
    Info,
    Malla,
    Codigo
  },

  props:['mallaAlumno'],
  data () {
    return{
      valido:true
    }
  },
  methods: {
        actualizar: function() {
          setTimeout(()=>{this.valido = true;},3000)
          
        }
      },
  
};

</script>