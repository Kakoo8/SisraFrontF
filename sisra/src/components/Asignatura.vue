<template>
    
        
        <div class='card'>
                {{asign}}
        
        </div>
    
     
</template>

<style>

</style>

<script>
export default{

props:['asignatura'],
data: function () {
  return {
    asign: this.asignatura
  }
}        
}

</script>