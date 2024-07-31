<template>
  <div>
    <h1 class="header">Hello World!</h1>
    
    <Component01 />
    <Component02 />
    <Component05 />
    <Component06 />
    <Component07 />
  </div>
</template>

<script>
  import Component01 from './components/Component01.vue'
  import Component02 from './components/Component02.vue'
  import Component05 from './components/Component05.vue'
  import Component06 from './components/Component06.vue'
  import Component07 from './components/Component07.vue'
  
  export default {
    name: 'App',
    components: {
      Component01,
      Component02,
      Component05,
      Component06,
      Component07,
    } 
  }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: #35495e;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>