<template>
  
  <div class="columns ">
  
  <div v-for ="(nivel,indice) in info">

    <div class="column" id="nivel">
                NIVEL {{indice +1}}
                
                <div  v-for ="asignatura in nivel" >
                  
                  <div  class="card" card-shadow=5px v-if="asignatura.situacion=='A'" id="asignatura">
                    
                      {{asignatura.nombreAsig}}
                      <br>
                      
                      <div id = "estrellas" v-if="asignatura.peso>-1">
                        <div v-for="n in asignatura.peso" >
                      <img id="estrella" src="../assets/estrella.png" width="20px" height="20px">
                        </div>
                      </div>  
                  </div>
                  <div  class="card" v-else id="asignatura2">
                    
                      {{asignatura.nombreAsig}}
                      <br>
                      
                      
                      <div id = "estrellas" v-if="asignatura.peso>-1">
                        <div v-for="n in asignatura.peso" >
                      <img id="estrella" src="../assets/estrella.png" width="20px" height="20px">
                        </div>
                      </div>  
                    
                  </div>        
                  <br>
                </div>

              </div>

  </div>
                 

  </div>
                
</template>

<style >
#padre{
  overflow:none;
  max-height: 100%;
  max-width: 100%;
  background-color: transparent;
  
  
}



#nivel{
  background-color:transparent;
  color: black;
  
  
}
#estrella{
  float: left;
  
}
#estrellas{
  display: flex;
  justify-content: center;
  padding-left: 0px;
}
#asignatura{

  max-height: 110px;
  min-height: 110px;
  max-width: 110px;
  min-width: 110px;
  background-color:green;
  color:white;
  text-align: center;
  align-content: center;
  -webkit-box-shadow: 10px 10px 17px -1px rgba(0,0,0,0.75);
  -moz-box-shadow: 10px 10px 17px -1px rgba(0,0,0,0.75);
  box-shadow: 10px 10px 17px -1px rgba(0,0,0,0.75);
  font-size:10px;
  padding: 10px;
  
  
}

#asignatura2{
  max-height: 110px;
  min-height: 110px;
  max-width: 110px;
  min-width: 110px;
  background-color:yellow;

  color:black;
  text-align: center;
-webkit-box-shadow: 10px 10px 17px -1px rgba(0,0,0,0.75);
-moz-box-shadow: 10px 10px 17px -1px rgba(0,0,0,0.75);
box-shadow: 10px 10px 17px -1px rgba(0,0,0,0.75);
  font-size:10px;
  padding: 10px;
}
.column{
  display: flex;
  flex-direction: column;
  align-items:center;
  
  background-color:transparent;
}

</style>

<script>
import Asignatura from './Asignatura.vue'

export default {
  Asignatura,

props:["info"],

  
data () {
  return{


}
} 

}

</script>