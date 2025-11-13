<script setup lang="ts">

defineProps<{
  title: string;
  url: string;
  img: string;
  loaded: boolean;
}>();

const closeTab = () => {
  console.log('Close tab clicked');
};


</script>
<template>
  <a :href="url" target="_blank">
    <div id="background">
      <div id="tab-image">
        <img :src="img" alt="Tab Image" v-if="loaded" />
      </div>
      <div id="tab-info">
        <h3>{{ title }}</h3>
        <p>{{ url }}</p>
      </div>
      <div id="closeTab" @click="closeTab">x</div>
  </div>
</a>
  </template>

<style scoped>

div#background {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: var(--padding-primary);
  border-radius: var(--radius-primary);
  background-color: var(--color-background);
}
div#background:hover{
  border: 1px solid #ccc;

}

a {
  display: block;
  padding: 0;
  margin:0;
}

#tab-image img {
  width: 50px;
  height: 50px;
  object-fit: cover;
  border-radius: 5px;
  color: var(--color-subtext);
}

#tab-info p {
  color: var(--color-subtext);
  font-size: x-small;
}

#tab-info {
  flex-grow: 1;
  margin-left: 15px;
}

div#closeTab {
  cursor: pointer;
  text-align: center;
  width: 35px;
  color: var(--danger-primary);
  padding: var(--padding-secondary);
  border-radius: var(--radius-secondary);
  font-weight: bold;
}
div#closeTab:hover {
  background-color: var(--color-background-mute);
}



</style>
