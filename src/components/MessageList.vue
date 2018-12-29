<template>
  <div class="messageContainer">
    <div class="topMessageContainer"></div>
    <hr color="#e7e7e7" size="1px">
    <div class="messageContainerEdit">
      <div>
        <img src="..//assets/meh.png"/>
      </div>
      <textarea></textarea>
    </div>
  </div>
</template>


<script>
export default {
  name: "MessageList",
  data() {
    return {};
  }
};
</script>


<style>
.messageContainer {
  height: 100%;
  width: 75%;
  background-color: #f2f2f2;
}

.topMessageContainer {
  height: 70%;
  width: 100%;
}

.messageContainerEdit {
  height: 29.9%;
  width: 100%;
  background-color: white;
}

textarea {
  box-sizing: border-box;
  padding: 0 30px;
  height: 20%;
  width: 100%;
  border: none;
  outline: none;
  font-family: Micrsofot Yahei;
  resize: none;
}

img{
  width: 4%;
  padding: 10px;
  margin-left: 20px;
}
</style>
