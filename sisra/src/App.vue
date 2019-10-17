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
                  Nombre Alumno: Claudio Urrutia
                </p>
                <p class="level-item has-text-centered">
                  Carrera: Ingenieria en Ejecución Informática
                </p>
                <p class="level-item has-text-centered">
                  
                </p>
                <p class="level-item has-text-centered">
                  
                </p>
                <p class="level-item has-text-centered">
                <input class="input is-warning" type="text" placeholder="Ingrese Rut">
                  
                </p>
              </nav>
        
      
      </h2>

    </div>
 
       
      
      
  
    <div class="container2">
      
        <div class="column " id="malla">
          <Malla v-bind="mallaAlumno"></Malla>

        </div>
        <!--<div class="column">
          <Codigo/>
          <br>
          <Info/>
        </div>
        -->
        </div>
      
    
  

     </div>
</template>

<style>

.section {
  display: flex;
  
  background-color: gray;
  padding: 1rem 1.1rem;
  max-height: 200px;
}

.container2{
  display: flex;
  
  width:100%;
  max-height:100%;
  min-height:100%;
  background-color: gray;
}
#app {
  
  height: 100%;
  max-width: 100%;
  
  

  
}
  html, body {
    margin: 0;
    height: 100%;
    max-height:100%;
  min-height:100%;
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
  data: () => ({
    //
  }),
};
</script>