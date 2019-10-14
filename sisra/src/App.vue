<template>
  <v-app>
  <nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item" >
      <img src="https://www.usach.cl/sites/default/files/logo_usach.jpg" width="112" height="28">
    </a>


  </div>

  <div id="navbarBasicExample" class="navbar-menu">
    <div class="navbar-start">
      <a class="navbar-item">
        
      </a>

      <a class="navbar-item">
        
      </a>

     

        
          <a class="navbar-item">
            Nombre Alumno:
          </a>
          <a class="navbar-item">
            Carrera:
          </a>
          <a class="navbar-item">
            
          </a>
          <hr class="navbar-divider">

        
      
    </div>

    <div class="navbar-end">
      <div class="navbar-item">
        <input class="input is-warning" type="text" placeholder="Ingrese Rut">
      
      </div>
    </div>
  </div>
</nav>
    <body>
  <section class="section">
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
  </section>
</body>
  </v-app>
</template>

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
