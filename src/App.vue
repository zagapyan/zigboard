<template>
  <div id="app">
    <ZigBoard v-bind:title="title" v-bind:sounds="sounds"/>
  </div>
</template>

<script>
import ZigBoard from './components/ZigBoard.vue'
import soundData from './assets/sound-data.json'
export default {
  name: 'app',
  components: {
    ZigBoard
  },
  data: ()=>({
    title: 'ZigBoard',
    sounds: soundData
  })
}
</script>

<style>
html{
  padding: 0;
  margin: 0;
  background: linear-gradient(45deg, #d26ac2, #46c9e5);
}
body{
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #000;
  background: #000;
  margin: 5px;
  padding: 20px;
  border-radius: 4px;
}
</style>
