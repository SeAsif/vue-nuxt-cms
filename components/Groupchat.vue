<template>
  <div class="h-100">
    <div class="groupchat-sidebar">
      <div class="chat-box">
        <h2 class="m-0">Chat</h2>
        <b-button variant="primary"
          ><img src="~assets/i/cross-black.png"
        /></b-button>
      </div>

      <div class="group-box">
        <b-button variant="primary"
          ><img src="~assets/i/arrow2-back.svg"
        /></b-button>
        <div class="text-box text-center">
          <h5>Group Chat</h5>
          <p>11 members</p>
        </div>
      </div>

      <div class="flex-msg-box2 h-100">
        <div class="messages-box">
          <div class="forword-msg">
            <p>Hey What’s up man?<span class="time">5:20 PM</span></p>
            <p>
              <strong>Vasilii Kovalchuk</strong> How u doing? Do u wanna change
              some bitcoins?<span class="time">5:20 PM</span>
            </p>
          </div>
          <div class="in-msg">
            <p>
              Yeah man! I need to change 895 BTC. Do you have it in your pocket
              =) ?<span class="time">5:20 PM</span>
              <strong>Read</strong>
            </p>
          </div>

          <div class="forword-msg">
            <p>
              <strong>Vasilii Kovalchuk</strong> Of course, I have. And do you
              have money to buy them?<span class="time">5:20 PM</span>
            </p>
          </div>
        </div>

        <div class="enter-message">
          <b-form>
            <b-form-input
              id="inline-form-input-name"
              placeholder="Enter Message ..."
            ></b-form-input>
            <div class="send-box">
              <b-button variant="primary">
                <b-img src="~assets/i/view.svg" />
              </b-button>
              <b-button variant="primary">
                <b-img src="~assets/i/simail.svg" />
              </b-button>
              <b-button variant="primary" class="send">
                Send
              </b-button>
            </div>
          </b-form>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.chat-box {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px 20px 16px 15px;
}
.chat-box h2 {
  font-weight: normal;
  font-size: 24px;
  color: #212121;
}
.groupchat-sidebar .chat-box {
  border-bottom: 1px solid #e5e9ee;
}
.groupchat-sidebar button {
  background: none;
  border: 0;
}
.groupchat-sidebar button:hover {
  background: none;
}
.groupchat-sidebar button:focus {
  box-shadow: none;
}
.groupchat-sidebar button img {
  width: 18px;
}
.group-box {
  display: flex;
  justify-content: center;
  break-after: column;
  background: #f9f9f9;
  position: relative;
  padding: 12px 0;
}
.group-box h5 {
  font-weight: 500;
  font-size: 14px;
  margin: 0;
}
.group-box p {
  color: #b4b4b4;
  font-weight: bold;
  font-size: 10px;
  margin: 0;
}
.group-box button img {
  width: 8px;
}
.group-box button {
  position: absolute;
  left: 12px;
  top: 8px;
}
</style>
