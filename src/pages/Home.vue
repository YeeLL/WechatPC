<template>
  <div class="container">
    <LeftView/>
    <router-view class="right"></router-view>
  </div>
</template>


<script>
import LeftView from "../components/LeftView.vue";
export default {
  components: {
    LeftView
  }
};
</script>


<style>
.container {
  margin-top: 20px;
  width: 800px;
  height: 600px;
  background-color: rebeccapurple;
  display: flex;
  flex-direction: row;
}

</style>

