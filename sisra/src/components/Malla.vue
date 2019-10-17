<template>
<div class="card">
  <div class="columns is-desktop">
  
              <div class="column">
                NIVEL 1
                <div  v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_cod}}
                  ______________________
                  <br>
                  {{asignatura.asi_nom}}
                  <br>
                 </div>

              </div>
              <div class="column">
                <div  v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                 
                </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                 </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                 </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                 </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">
                  {{asignatura.asi_nom}}
                  <br>
                </div>

              </div>
              <div class="column">
                <div class="card" v-for ="asignatura in asignaturas" v-bind:key="asignatura">

                  {{asignatura.asi_nom}}
                  <br>
                </div>

              </div>                                          

  </div>
</div>                    
</template>

<style >
.card{
  overflow:scroll;
  max-height: 100%;
  
}
.table{
      max-width:10px ;
      border: 2px solid black;
      border-collapse: inherit;

}
.card::-webkit-scrollbar {
    display: none;
}
table, th, td {
  border: 1px solid black;
  
}

#malla{
  display:flex;
  flex-direction: row;
}
.column{
  display: flex;
  flex-direction: column;
  align-items:center;
}
</style>

<script>
import Asignatura from './Asignatura.vue'

export default {
    Asignatura,


  
data () {
  return{
  "asignaturas":
    [
      {"asi_cod":13273,
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
       "asi_sct":0
      },
      {"asi_cod":13277,
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
       "asi_sct":0
      },
      {"asi_cod":13276,
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
       "asi_sct":0
      },
      {"asi_cod":13270,
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
       "asi_sct":0
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
       "asi_sct":0
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
       "asi_sct":0
      },
      
    ]
}
} 

}

</script>