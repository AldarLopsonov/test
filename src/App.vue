<template>
    <TheHeader />
    <TheMain />
    <TheFooter />
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheMain from './components/TheMain.vue';
import TheFooter from './components/TheFooter.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheMain,
    TheFooter
}
}
</script>

<style>

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

hr {
  border: 1px solid rgba(14, 95, 173, 0.3);
  ;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: white;
  min-width: 1439px;
  max-width: 1440px;
  height: fit-content;
}

.container {
  display: flex;
  height: 100%;
  margin: 0 200px;
}

a {
  text-decoration: none;
  color: white;
}


</style>
