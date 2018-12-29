<template>
  <div class="ContactContainer">
    <div class="ContactContainerScroll">
      <ul>
        <li v-for="(item,position) in items" :key="item.id">
          <div
            :class="item.sessionClass"
            @click="itemClic(position)"
            @mouseover="enter(position)"
            @mouseout="leave(position)"
          >
            <img src="..//assets/head.jpg">
            <div class="sessionRight">
              <span class="sessionName">{{ item.name }}</span>
              <span class="sessionTime">{{item.time}}</span>
              <p>{{item.content}}</p>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>


<script>
var currentItemPosition = 0;
var entryItemPosition = 0;
export default {
  name: "contact",
  data() {
    return {
      items: [
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "sessionSelect"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        },
        {
          icon: "",
          name: "加菲",
          content: "置顶asdfasdaaafsadf聊天",
          time: "14:40",
          sessionClass: "session"
        }
      ]
    };
  },
  methods: {
    itemClic: function(position) {
      this.items[currentItemPosition].sessionClass = "session";
      this.items[position].sessionClass = "sessionSelect";
      currentItemPosition = position;
    },
    enter: function(position) {
      if (position != currentItemPosition) {
        this.items[position].sessionClass = "sessionOver";
        entryItemPosition = position;
      }
    },
    leave: function(position) {
      if (position != currentItemPosition) {
        this.items[position].sessionClass = "session";
      }
    }
  }
};
</script>


<style scoped>
.ContactContainer {
  width: 25%;
  height: 100%;
  overflow: hidden;
  background-color: #e6e6e6;
}

.ContactContainerScroll {
  width: 109%;
  height: 100%;
  overflow: auto;
}
.sessionOver {
  display: inline-flex;
  background-color: #d9d9d9;
}
.sessionSelect {
  display: inline-flex;
  background-color: #c4c4c4;
}

img {
  padding: 10px;
  width: 20%;
  height: 20%;
}
.session {
  display: inline-flex;
  background-color: #e6e6e6;
}

.sessionRight {
  width: 80%;
  position: relative;
  margin-top: 10px;
  display: inline-block;
  align-items: flex-end;
}

.sessionName {
  font-size: 15px;
  color: black;
}

.sessionTime {
  right: 9%;
  position: absolute;
  margin-top: 5px;
  color: #9999ad;
  font-size: 12px;
}

p {
  width: 80%;
  margin-top: 6px;
  font-size: 13px;
  display: block;
  overflow: hidden;
  text-overflow: ellipsis;
  color: #9999ad;
  white-space: nowrap;
}
</style>
