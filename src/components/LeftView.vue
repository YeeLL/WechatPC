<template>
  <div class="left_content">
    <img src="../assets/head.jpg" alt="头像" class="head">
    <div class="mid">
      <img src="../assets/chat_enable.png" alt="聊天" class="chat" @click="toggle($event)">
      <img src="../assets/contact.png" alt="联系人" class="contact">
      <img src="../assets/meh.png" alt="我自己" class="me">
    </div>
    <img src="../assets/menu.png" alt="菜单" class="footer">
  </div>
</template>


<script>
export default {
  name: "leftview",
  data() {
    return {
      headIcon: "../assets/head.jpg",
      chatIcon: "../assets/chat_enable.png",
      contactIcon: "../assets/contact.png",
      mehIcon: "../assets/meh.png"
    };
  },
  methods: {
    toggle: function(alt) {
      console.log(alt.toElement.alt);
      alt.toElement.alt = "jaajjaja";
      console.log(alt.toElement.alt);
      alt.toElement.src = this.mehIcon;
    }
  }
};
</script>


<style>
.head {
  margin-top: 20%;
  margin-right: 10%;
  margin-left: 10%;
  width: 80%;
}
.footer {
  width: 60%;
  margin-left: 20%;
  position: absolute;
  bottom: 5%;
}
.chat {
  width: 60%;
}
.contact {
  margin-top: 10%;
  width: 60%;
}
.me {
  margin-top: 10%;
  width: 60%;
}
.mid {
  margin-left: 20%;
  margin-top: 25%;
}

.left_content {
  width: 100%;
  position: relative;
  background-color: #2b2c2f;
  height: 100%;
}
</style>
