<template>
  <div class="container">
    <div class="leftbox">
      <LeftView/>
    </div>
    <div class="rightBox">
      <Header></Header>
      <hr color="#e7e7e7" size=1px/>
      <div class="contactBox">
        <Contact/>
        <MessageList/>
      </div>
    </div>
  </div>
</template>


<script>
import LeftView from "../components/LeftView.vue";
import Header from "../components/SearchHead";
import Contact from "../components/Contact";
import MessageList from "../components/MessageList";

export default {
  components: {
    LeftView,
    Header,
    Contact,
    MessageList
  }
};
</script>


<style>
.container {
  margin-top: 20px;
  width: 1000px;
  height: 650px;
  display: flex;
  flex-direction: row;
}

.leftbox {
  width: 7.5%;
}

.rightBox {
  display: flex;
  width: 100%;
  flex-direction: column;
}

.contactBox {
  background: #e6e6e6;
  width: 100%;
  height: 89.5%;
  display: flex;
  flex-direction: row;
}

li{
  list-style: none;
}
</style>

