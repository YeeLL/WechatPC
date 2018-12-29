<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  width: 100%;
  height: 100%;
  background: linear-gradient(#b7b3b2, #303c48);
  background-size: 100% 100%;
  position: fixed;
  display: flex;
  justify-content: center;
}

* {
  padding: 0px;
  margin: 0px;
}
</style>
