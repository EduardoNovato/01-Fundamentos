<script>

export default {
  data: () => ({
    contador: 0
  }),
  methods: {
    contar(){
      this.contador++
    },
    noContar(){
      this.contador--
    },
    resert(){
      this.contador = 0
    }
  }
}


</script>
<template>
  <div class="container">
    <img src="./assets/chayanne.jpg" alt="" height="275" width="235" />
    <h1>Hola carambola la run run</h1>

    <hr />

    <h2 class="h2">Contador: {{contador}}</h2>
    <button class="button" @click="contar()">+1</button>
    <button class="button" @click="noContar()">-1</button>
    <button class="button" @click="resert()">Resest</button>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
}

.h2 {
  font-size: 2.5rem;
}
.button {
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 6px;
}
</style>