<script setup>
import { ref } from 'vue';

defineProps({
    data: String
});

const header = ref('to do items')
const items = ref([
{id:1, level :'this is fun'},
{id:2, level :'this is fun'},
{id:3, level :'this is fun'},
])



</script>

<template>
  
    <div>
        <h3>{{ header }}</h3>
    <ul className="arrey">
        <li v-for="(item,id) in items" :key="id" >
           ---{{ item.level }}-- {{item.id}} 
        </li>
    </ul>
    <h2>{{ data }}</h2>

    </div>

</template>
<style scoped>
.arrey{
    color: red;
    list-style: none;
   
}
</style>