<template>
  <div class="left_content">
    <header>
      <img src="../assets/head.jpg" alt="头像" class="head">
    </header>
    <div class="mid">
      <img src="../assets/chat_enable.png" alt="聊天" class="chat">
      <img src="../assets/contact.png" alt="联系人" class="contact">
      <img src="../assets/meh.png" alt="我自己" class="me">
    </div>

    <footer>
      <img src="../assets/menu.png" alt="菜单" class="footer">
    </footer>
  </div>
</template>


<script>
export default {
  name: "leftview"
};
</script>


<style>
.chat {
  margin-top: 25px;
  width: 30px;
  height: 30px;
}
.me {
  margin-top: 15px;
  width: 27px;
  height: 27px;
  margin-left: -2px;
}
.contact {
  margin-top: 12px;
  width: 30px;
  height: 30px;
}
.mid {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.head {
  width: 40px;
  height: 40px;
}
.footer {
  width: 40px;
  height: 40px;
  margin-bottom: 20px;
}
.left_content {
  width: 70px;
  padding-top: 20px;
  background-color: #434447;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
</style>
