
<script setup lang="ts">
import TabCard from '@/components/list/TabCard.vue';
import { ref } from 'vue';

const items = ref([
  {title:"eee", url:"https://google.com",img:"image.png", loaded:true},
  {title:"rrr", url:"https://bing.com",img:"image2.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
  {title:"ttt", url:"https://duckduckgo.com",img:"image3.png", loaded:true},
]);

</script>

<template>
<main>
<span v-for="(item, index) in items" :key="index">
  <TabCard :title="item.title" :url="item.url" :img="item.img" :loaded="item.loaded" />
</span>
</main>

</template>
