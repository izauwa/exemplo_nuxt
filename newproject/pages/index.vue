<template>
  <div class="container">
    <h1>{{titulo}}</h1>
    <ul>
      <li :key="item.id" v-for = "item in pessoas">
      </li>
    </ul>
    <button @click="digaOla">Diga olá!</button>
    </div>

</template>

<script>
export default {
  data: function(){
    return{
      titulo:"Lista de pessoas e idade",
      pessoas: [
        {id: 1, nome: "Marcio", idade:"33"},
        {id: 2, nome: "Diego", idade:"44"},
        {id: 3, nome: "Launa", idade:"50"},
        {id: 4, nome: "Tamara", idade:"23"},

    ]

    }
  } ,
  methods:{
    digaOla: function(){

      alert("Olá Mundo do Nuxt.js!");

    }


    }


  }
 

</script>

<style scoped>

.container{

  margin: 20px

}
</style>
