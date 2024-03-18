<script setup>
import { ref } from 'vue'
defineProps({
  msg:String,
})
const count = ref(0)
</script>

<template>
  <div>
  <h1>{{ msg }}</h1>
 

  <div class="card">
    <button class="buton1" type="button" @click="count++">+ </button><br>
    <button class="buton1" type="button" v-if="count > 0" @click="count--">-</button>
    <h4>{{ count }}</h4>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p>
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>
  <p>
    Install
    <a href="https://github.com/vuejs/language-tools" target="_blank">Volar</a>
    in your IDE for a better DX
  </p>
 
</div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
.buton1{
  padding-bottom: 10px;
  margin-top: 30px;
}
</style>
