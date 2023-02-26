<script setup>
import MinhaApp from './components/MinhaApp.vue'
</script>

<template>
  <header>
    <h3> Unifor - ADS - Desenvolvimento de software em nuvem</h3>

    <div class="wrapper">
      <MinhaApp msg="Deu certo!" />
    </div>
  </header>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
