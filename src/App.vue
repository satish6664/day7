<template>
  <div>
    <CounTer />
    <div>
      <span>App: </span>{{ $store.state.count }}
    </div>
  </div>
</template>

<script setup>
import CounTer from './components/CounTer.vue';
</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align:justify;
  color: #0c80f5;
  margin-top: 60px;
}
</style>
