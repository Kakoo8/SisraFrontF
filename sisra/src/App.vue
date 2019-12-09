<template>

  <div id="app" >
     <b-navbar fixed-top shadow> 
        <template slot="brand">
            <b-navbar-item tag="div">
                  <img src="http://en.usach.cl/sites/default/files/logo-usach_2.png" width="40" height="auto">
                  SISRA  

            </b-navbar-item>
        </template>
        <template slot="start">
            <b-navbar-item tag="div">
                
            </b-navbar-item>
            <b-navbar-item tag="div">
              
                Alumno: {{info.data.datosAlumno.nombreAlu}} {{info.data.datosAlumno.paternoAlu}} {{info.data.datosAlumno.maternoAlu}}
                
            </b-navbar-item>
            
        </template>

        <template slot="end">
            <b-navbar-item tag="div">
                <input class="input is-warning" type="text" v-model="rut" v-on:keyup.enter="cargarDatos()" placeholder="Ingrese Rut">

            </b-navbar-item>
        </template>
    </b-navbar>
  
    
    <div class="container">
      <div class="subtitle">
      <div class="level">
                <div class="level-item">
                {{info.data.datosAlumno.tipoCarrera}} {{info.data.datosAlumno.especialidadCarrera}}
                </div>
                <div class="level-item">
                 Información
                </div>
                
                
              </div>
        
      
      </div>

    </div>
 
       
      
      
  
    <div class="container is-fluid" id="container2">
      
          <Malla :info="info.data.malla" ></Malla>
          

    </div>
        <!--<div class="column">
        <div class="column " id="malla" >
          <Codigo/>
          <br>
          <Info/>
        </div> is-four-fifths-->



   
    </div>
      
    
  

     
</template>

<style>

.section {
  display: flex;
  
  background-color: gray;
  padding: 1rem 1.1rem;
  
}

.navbar.is-fixed-top {
    left: 0px;
    position: fixed;
    right: 0px;
    z-index: 30;
    top: 0px;
    background-color:#005190;
    color: #ffffff !important;
}
.container{
  font-size: 14px;
  font-size-adjust: inherit;
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
    background-color: #ffffffe5; 
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
import axios from 'axios';
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
      valido:true,
      info:{data:{
            datosAlumno:{},

      }},
      rut:null
    }
  },
  methods:{
          cargarDatos() {
          axios
          .get('http://localhost:3001/asignaturas_importantes/buscarAlumnoPorRut/'+ this.rut)
          .then(response => (this.info = response))
          }

  },
  mounted () {

  }
};

</script>