<template>

  <div id="app" style="min-height: 100vh" >
     <b-navbar fixed-top color=white> 
        <template slot="brand">
            <b-navbar-item tag="div">
                  <img src="http://en.usach.cl/sites/default/files/logo-usach_2.png" width="auto" height="auto">
                  SISRA  

            </b-navbar-item>
        </template>
        <template slot="start">
            <b-navbar-item tag="div">
                
            </b-navbar-item>
            <b-navbar-item tag="div" v-show="cargado">
              
                Alumno: {{info.data.datosAlumno.nombreAlu}} {{info.data.datosAlumno.paternoAlu}} {{info.data.datosAlumno.maternoAlu}}
                
            </b-navbar-item>

            
        </template>

        <template slot="end">
            <b-navbar-item tag="div">
                <input class="input is-warning" type="text" v-model="rut" v-on:keyup.enter="cargarDatos()" placeholder="Ingrese Rut">
                 <b-button type="is-warning" v-on:click="cargarDatos()">Buscar</b-button>
                 <b-button id="informacion" rounded @click="alertCustom" ><img src="./assets/question.png" width="auto" height="auto"></b-button>
            </b-navbar-item>
        </template>
    </b-navbar>
  
    
    <div class="container" id="botones" v-show="cargado" >
              
            
                
 
      <div class="subtitle">
                  CARRERA: {{info.data.datosAlumno.tipoCarrera}} {{info.data.datosAlumno.especialidadCarrera}}
                  <br>
                  PPA: {{info.data.datosAlumno.ppa}}  NAS: {{info.data.datosAlumno.nas}}  NAR: {{info.data.datosAlumno.nar}}


        
      
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
    height: 0px;  
    background: rgba(0,58,102,1);
    background: -moz-linear-gradient(top, rgba(0,58,102,1) 0%, rgba(0,58,102,1) 80%, rgba(22,141,177,1) 95%, rgba(4,42,58,1) 100%, rgba(4,42,58,1) 100%);
    
    background: -webkit-linear-gradient(top, rgba(0,58,102,1) 0%, rgba(0,58,102,1) 80%, rgba(22,141,177,1) 95%, rgba(4,42,58,1) 100%, rgba(4,42,58,1) 100%);
    background: -o-linear-gradient(top, rgba(0,58,102,1) 0%, rgba(0,58,102,1) 80%, rgba(22,141,177,1) 95%, rgba(4,42,58,1) 100%, rgba(4,42,58,1) 100%);
    background: -ms-linear-gradient(top, rgba(0,58,102,1) 0%, rgba(0,58,102,1) 80%, rgba(22,141,177,1) 95%, rgba(4,42,58,1) 100%, rgba(4,42,58,1) 100%);
    background: linear-gradient(to bottom, rgba(0,58,102,1) 0%, rgba(0,58,102,1) 80%, rgba(22,141,177,1) 95%, rgba(4,42,58,1) 100%, rgba(4,42,58,1) 100%);
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#003a66', endColorstr='#042a3a', GradientType=0 );

   
    

    
   

}
.navbar-item {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    color: 
    white !important;
}
.navbar-item{
  color: #ffffff;
}
.level-item,#botones{
  justify-content: left;
  
  font-size: 14px;
  font-size-adjust: inherit;
  text-align: left;
  background-color:transparent;
}

#container2{
  display: flex;
  width: -webkit-fill-available;
  
  min-height: 100%;
  max-height: 100%;
  background-color: transparent;
  
}
#informacion{
  background-color: transparent;
  color:white;
  border-color: transparent;
}
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    background-color: #ffffffe5;
    background-image: url("./assets/logo_usach.jpg");
     
    
    
    background-position:center;
    color: #ffffff;
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
  color:black;
   
 } 
 #botones{
   border-bottom-style: groove;
 }



</style>
<script>


import Malla from './components/Malla';
import axios from 'axios';
export default {
  name: 'App',
  components: {
    
    
    Malla
  
  },

  props:['mallaAlumno'],
  data () {
    return{
      isActive:false,
      valido:true,
      cargado:false,
      loading:true,
      errored:false,
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
          .catch(error => {
          
          
          this.cargado= false
          })
          .then(response => (this.info = response),this.cargado=true)
          .finally(() => this.loading = false)
          
          },
          alertCustom() {
                this.$buefy.dialog.alert({
                    title: 'INFORMACIONES',
                    message: '¿Que son PPA, NAS y NAR? \n PPA:es esto \n NAS:es esto \n NAR: es esto. ',
                    confirmText: 'Listo'
                    
                })
            },

  },
  mounted () {

  }
};

</script>