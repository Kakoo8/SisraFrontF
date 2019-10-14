<template>
  <v-app>
  <section class="section" heigth="30px">
    
    <div class="container">
      <h1 class="title">
      <nav class="level">
          <p class="level-item has-text-centered">
            <img src="https://www.usach.cl/sites/default/files/logo_usach.jpg" width="200" height="auto">
          </p>
          <p class="level-item has-text-centered">
            
          </p>
          <p class="level-item has-text-centered">
            
          </p>
          <p class="level-item has-text-centered">
            
          </p>
          <p class="level-item has-text-centered">
           
            
          </p>
        </nav>
      
      </h1>
      <h2 class="subtitle">
       <nav class="level">
          <p class="level-item has-text-centered">
            Nombre Alumno:
          </p>
          <p class="level-item has-text-centered">
            Carrera: 
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
  </section>
  
       
      
   <body>   
  
    <div class="container">
      <div class="columns">
        <div class="column is-four-fifths">
          <Malla/>

        </div>
        <div class="column">
          <Codigo/>
          <br>
          <Info/>
        </div>

        </div>
      </div>
    </div>
  
</body>
  </v-app>
</template>

<style>
.section {
    padding: 1rem 1.1rem;
}
</style>
<script>
import HelloWorld from './components/HelloWorld';
import Codigo from './components/CodigoColor';
import Info from './components/Info';
import Malla from './components/Malla';
export default {
  name: 'App',
  components: {
    HelloWorld,
    Info,
    Malla,
    Codigo
  },
  data: () => ({
    //
  }),
};
</script>