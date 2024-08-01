<script setup>
  // vue：將需要的「方法」用 import 的方式取用進來
  import { ref } from 'vue';

  const num = ref(1);

  function clickMe() {
    num.value ++
  }

  // return{} => 在 vue 的 <script setup> 不需撰寫 ; cdn 的 setup() {} 需要 
</script>

<template>
  <div>
    {{ num }}
  
    <button type="button" v-on:click="clickMe">點我</button>
  </div>
</template>

