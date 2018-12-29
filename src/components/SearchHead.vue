<template>
  <div class="header">
    <div class="left">
      <div class="searchBox">
        <input type="text" placeholder="搜索">
        <img src="..//assets/search.png">
      </div>
      <!-- searchBox -->
    </div>
    <!-- left end -->
    <div class="right">
      <p>一心</p>
    </div>
    <!-- right edn -->
  </div>
</template>

<script>
export default {
  name: "header",
  data() {
    return {
      name: "新的朋友"
    };
  }
};
</script>


<style scoped>
.header {
  position: relative;
  display: flex;
  width: 100%;
  height: 10.5%;
  flex-flow: row;
  background-color: #f2f2f2;
}

.left {
  width: 25%;
  display: inline-flex;
  justify-content: center;
  position: relative;
  background-color: #e6e6e6;
}
.right {
  display: flex;
  align-items: flex-end;
  padding-bottom: 10px;
  padding-left: 20px;
}

.right p {
  font-size: 25px;
}

.searchBox {
  display: inline-flex;
  position: relative;
  top: 40%;
  height: 35%;
  border-width: 2px;
  border-color: #d9d7d6;
  border-style: solid;
  background-color: #e5e3e2;
}

.searchBox input {
  padding-left: 10px;
  background-color: #e5e3e2;
  border-style: none;
  outline: none;
}

.searchBox img {
  width: 20px;
  height: 20px;
  margin-top: 2px;
}

* {
  padding: 0px;
  margin: 0px;
}
</style>
