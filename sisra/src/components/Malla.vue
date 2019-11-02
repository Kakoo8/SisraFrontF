<template>

  <div class="columns ">
  
              <div class="column">
                NIVEL 1
                
                <div  v-for ="asignatura in nivel1" >
                  <div class="card" id="asignatura">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} <br> {{asignatura.asi_peso}}</h6>
                    </div>
                  </div> 
                  <br>
                 </div>

              </div>
              <div class="column">
                NIVEL 2
                
                <div  v-for ="asignatura in nivel2" >
                  <div class="card" id="asignatura">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} {{asignatura.asi_peso}}</h6>
                    </div>
                  </div>    
                  <br>
                </div>

              </div>
              <div class="column">
                NIVEL3
                
                <div  v-for ="asignatura in nivel3" >
                  <div class="card" id="asignatura">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} {{asignatura.asi_peso}}</h6>
                    </div>
                  </div>
                  <br> 
                </div>

              </div>
              <div class="column">
              NIVEL 4
              
                <div  v-for ="asignatura in nivel4" >
                  <div class="card" id="asignatura">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} {{asignatura.asi_peso}}</h6>
                    </div>
                  </div>
                  <br> 
                </div>

              </div>
              <div class="column">
              NIVEL 5
              
                <div  v-for ="asignatura in nivel5" >
                  <div class="card" id="asignatura">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} {{asignatura.asi_peso}}</h6>
                    </div>
                  </div> 
                  <br>
                 </div>

              </div>
              <div class="column">
              NIVEL 6
              
                <div  v-for ="asignatura in nivel6" >
                  <div class="card" id="asignatura">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} {{asignatura.asi_peso}}</h6>
                    </div>
                  </div>
                  <br> 
                </div>

              </div>
              <div class="column">
              NIVEL 7
              
                <div  v-for ="asignatura in nivel7" >
                  <div class="card" id="asignatura2">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} {{asignatura.asi_peso}}</h6>
                    </div>
                  </div> 
                <br>
                </div>
              </div>
              <div class="column">
              NIVEL 8
                <div  v-for ="asignatura in nivel8" >
                  <div class="card" id="asignatura2">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} {{asignatura.asi_peso}}</h6>
                    </div>
                  </div> 
                <br>  
                </div>
              </div>
              <div class="column">
                <div  v-for ="asignatura in nivel9" >
                  <div class="card" id="asignatura">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} {{asignatura.asi_peso}}</h6>
                    </div>
                  </div> 
                 </div>
                 <br>
              </div>
              <div class="column">
                <div  v-for ="asignatura in nivel10" >
                  <div class="card" id="asignatura">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} {{asignatura.asi_peso}}</h6>
                    </div>
                  </div> 
                </div>
                <br>
              </div>
              <div class="column">
                <div  v-for ="asignatura in nivel11" >
                  <div class="card" id="asignatura">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} {{asignatura.asi_peso}}</h6>
                    </div>
                  </div> 
                </div>
                <br>
              </div>
              <div class="column">
                <div  v-for ="asignatura in nivel12" >
                  <div class="card" id="asignatura">
                    <div class="card-content">
                      <h6>{{asignatura.asi_nom}} {{asignatura.asi_peso}}</h6>
                    </div>
                  </div> 
                </div>
                <br>
              </div>
                                              

  </div>
                
</template>

<style >
#padre{
  overflow:none;
  max-height: 100%;
  max-width: 100%;
  
  
}
.table{
      max-width:10px ;
      border: 2px solid black;
      border-collapse: inherit;

}


.columns{
  background-color:gray;
  overflow:hide;
}
#asignatura{
  min-height:130px;
  max-height:130px;
  max-width:140px;
  min-width:140px;

  background-color:green;
  color:white;
  font-size:0.70em;
  overflow:hidden;
}
#asignatura2{
  min-height:130px;
  max-height:130px;
  max-width:140px;
  min-width:140px;
  background-color:yellow;
  color:black;
  font-size:12px;
}
.column{
  display: flex;
  flex-direction: column;
  align-items:center;
  
  background-color:white;
}
</style>

<script>
import Asignatura from './Asignatura.vue'

export default {
    Asignatura,


  
data () {
  return{
  
nivel1:[
       
      {"asi_cod":10126,
       "asi_nom":"MÉTODOS DE ESTUDIO",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10126",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":10125,
       "asi_nom":"INTRODUCCIÓN A LA INGENIERÍA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10125",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":10104,
       "asi_nom":"TALLER DE DESARROLLO PERSONAL E INTEGRAL",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10104",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":2
      },
      {"asi_cod":10102,
       "asi_nom":"ALGEBRA I PARA INGENIERÍA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10102",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":2
      },
      {"asi_cod":10101,
       "asi_nom":"CALCULO I PARA INGENIERÍA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10101",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":2
      },

      {"asi_cod":10103,
       "asi_nom":"FÍSICA I PARA INGENIERÍA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10108",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      }],
nivel2:[ 

      {"asi_cod":10108,
       "asi_nom":"ALGEBRA II PARA INGENIERÍA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10108",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":3
      },
            {"asi_cod":10110,
       "asi_nom":"FUNDAMENTOS DE COMPUTACIÓN Y PROGRAMACION",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10110",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":10109,
       "asi_nom":"FÍSICA II PARA INGENIERÍA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10109",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":2
      },
      {"asi_cod":10107,
       "asi_nom":"CALCULO II PARA INGENIERÍA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10107",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":6
      },
      {"asi_cod":10111,
       "asi_nom":"QUÍMICA GENERAL",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10111",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":0
      },
     ],
nivel3:[      {"asi_cod":10130,
       "asi_nom":"INGLÉS I",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10130",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":13201,
       "asi_nom":"MÉTODOS DE PROGRAMACIÓN",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13201",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":2
      },
      {"asi_cod":10128,
       "asi_nom":"COMUNICACIÓN EFECTIVA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10128",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":10127,
       "asi_nom":"ELECTRICIDAD Y MAGNETISMO PARA INGENIERÍA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10127",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":10123,
       "asi_nom":"ECUACIONES DIFERENCIALES Y MÉTODOS NUMÉRICOS PARA INGENIERÍA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10123",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":10115,
       "asi_nom":"ANÁLISIS ESTADÍSTICO PARA INGENIERÍA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10115",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      }
 ],

nivel4:[{"asi_cod":13273,
       "asi_nom":"ESTRUCTURA DE COMPUTADORES",
       "asi_teo":4,
       "asi_ejer":0,
       "asi_lab":2,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13273",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      }, 
           {"asi_cod":13252,
       "asi_nom":"INGENIERÍA DE SISTEMAS",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13252",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":13205,
       "asi_nom":"ANÁLISIS DE ALGORITMOS Y ESTRUCTURA DE DATOS",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13205",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":0
      },
      {"asi_cod":13204,
       "asi_nom":"PARADIGMAS DE PROGRAMACIÓN",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13204",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":2
      },
      {"asi_cod":10131,
       "asi_nom":"INGLÉS II",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10131",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":10116,
       "asi_nom":"FUNDAMENTOS DE ECONOMÍA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10116",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      }],
nivel5:[{"asi_cod":13275,
       "asi_nom":"ORGANIZACIÓN DE COMPUTADORES",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13275",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":2
      },
      {"asi_cod":13274,
       "asi_nom":"DISEÑO DE BASE DE DATOS",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13274",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":13261,
       "asi_nom":"SISTEMAS DE INFORMACIÓN",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13261",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":0
      },
      {"asi_cod":10128,
       "asi_nom":"INFORMÁTICA Y SOCIEDAD",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10128",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":10128,
       "asi_nom":"EVALUACIÓN Y GESTIÓN DE PROYECTOS",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10128",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":13209,
       "asi_nom":"FUNDAMENTOS DE INGENIERÍA DE SOFTWARE",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13209",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":10132,
       "asi_nom":"INGLÉS III",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10132",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      }],
nivel6:[ {"asi_cod":13266,
       "asi_nom":"REDES COMPUTACIONALES",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13266",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":13265,
       "asi_nom":"TÉCNICAS DE INGENIERÍA DE SOFTWARE",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13265",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":13262,
       "asi_nom":"ADMINISTRACIÓN Y GESTIÓN INFORMÁTICA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13262",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":13215,
       "asi_nom":"TALLER DE BASE DE DATOS",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13215",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":13212,
       "asi_nom":"SISTEMAS OPERATIVOS",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13212",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":10133,
       "asi_nom":"INGLÉS IV",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"10133",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      }],
nivel7:[{"asi_cod":13276,
       "asi_nom":"SEMINARIO DE COMPUTACIÓN E INFORMÁTICA",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13276",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      }, {"asi_cod":13270,
       "asi_nom":"TÓPICOS DE ESPECIALIDAD III",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13270",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":13269,
       "asi_nom":"TÓPICOS DE ESPECIALIDAD II",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13269",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":13268,
       "asi_nom":"TÓPICOS DE ESPECIALIDAD I",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13268",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      },
      {"asi_cod":13267,
       "asi_nom":"PROYECTO DE INGENIERÍA DE SOFTWARE",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13267",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":1
      }],
nivel8:[ {"asi_cod":13277,
       "asi_nom":"TRABAJO DE TITULACIÓN",
       "asi_teo":4,
       "asi_ejer":2,
       "asi_lab":0,
       "asi_tipo":"P",
       "asi_creg":1,
       "asi_elect":"N",
       "asi_vig":"S",
       "asi_cod_inge":"13277",
       "asi_titulo":"N",
       "asi_sct":0,
       "asi_peso":6,
      }],
nivel9:[],
nivel10:[],
nivel11:[],
nivel12:[],

}
} 

}

</script>