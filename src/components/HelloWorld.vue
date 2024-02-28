<template>
  <div>
    Hello World
   <h3> {{ info }} </h3> 
  </div>
    
</template>

<script>
export default {
  data(){
    return{
      info: 'Angel Emmanuel Cerda Reyna 20974 5A'
    }
  }
}
</script>

<style>
.content-center {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100px;
    text-align: center; 
   
}
</style>