<template>
    <div>
      <span>Hello</span>&nbsp;
      <button @click.prevent="update">Click</button>
      <h3>Component value: {{ counter }} & Store value: {{ $store.state.count }}</h3>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
import { useStore } from 'vuex';

  const store=useStore()
  function update(){
    store.commit('increase')
  }
  
  const counter = ref(0);
  </script>
  