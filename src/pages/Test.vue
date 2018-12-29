<template>
  <div class="box">
    <p>基金</p>
    <span>行内元素</span>
    <span>行内元素</span>
    <div class="posistion_fixed">
      hhhhhh
      哈哈哈哈哈
      <div class="box2">
       asdfasdf
       <input type = "text">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "test"
};
</script>


<style>
.box {
  height: 800px;
  width: 100%;
  background-color: black;
}
p {
  display: inline-block;
  background-color: antiquewhite;
}
span {
  display: inline-block;
  width: 200px;
  height: 200px;
  background-color: aqua;
}
.posistion_fixed {
  position: relative;
  left: 100px;
  height: 500px;
  background-color: aquamarine;
}
.box2 {
  display: inline-flex;
  color: black;
  border-color: brown;
  border-width: 2px;
  border-style: solid;
}
</style>
