<script>
export default {
  data() {
  
    var numeros = [
      (Math.floor(Math.random() * (99))),
      (Math.floor(Math.random() * (99))),
      (Math.floor(Math.random() * (99))),
      (Math.floor(Math.random() * (99))),
      (Math.floor(Math.random() * (99)))
    ]
    var maior = Math.max.apply(0, numeros);
    var menor = Math.min.apply(0, numeros);
 
    
    return {
      numeros: numeros,
      maior: maior,
      menor:menor
    }
  }
}
</script>

<template>
  <br/><br/>
  <div>
    <h5> Essa aplicação gera 5 números aleatórios, apresenta-os e informa o maior e menor número entre eles </h5> 
    
    <h5>Numeros: {{numeros}}</h5>
    <h5>Maior: {{maior}}</h5>
    <h5>Menor: {{menor}}</h5>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
