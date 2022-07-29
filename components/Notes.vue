<template>
  <div class="h-100">
    <div class="groupchat-sidebar">
      <div class="chat-box">
        <h2 class="m-0">Chat</h2>
        <b-button variant="primary"
          ><img src="~assets/i/cross-black.png"
        /></b-button>
      </div>

<div class="nots-flex">
<div class="nots-tabs">
<b-card no-body>
    <b-tabs card>
      <b-tab title="All Notes" active>
        <b-card-text>            <div class="messages-box">
              <div class="forword-msg">
                <p>
                  <b-form-checkbox
                    id="checkbox-1"
                    name="checkbox-1"
                    value="accepted"
                    unchecked-value="not_accepted"
                  >
                  </b-form-checkbox>
                  <strong>Vasilii Kovalchuk</strong>
                  <span class="h5">Home Page</span> One morning, when Gregor
                  Samsa woke from troubled dreams, he found himself transformed
                  <span class="time">(02:00 PM)</span>
                </p>
              </div>
              <div class="forword-msg">
                <p>
                  <b-form-checkbox
                    id="checkbox-2"
                    name="checkbox-3"
                    value="accepted"
                    unchecked-value="not_accepted"
                  >
                  </b-form-checkbox>
                  <strong>Vasilii Kovalchuk</strong>
                  <span class="h5">Team Page</span>"What's happened to me?" he
                  thought. It wasn't a dream. His room, a proper human room
                  although a little
                  <span class="time">(02:00 PM)</span>
                </p>
              </div>
              <div class="forword-msg">
                <p>
                  <b-form-checkbox
                    id="checkbox-3"
                    name="checkbox-3"
                    value="accepted"
                    unchecked-value="not_accepted"
                  >
                  </b-form-checkbox>
                  <strong>Vasilii Kovalchuk</strong>
                  <span class="h5">Team Page</span>A collection of textile
                  samples lay spread out on the table
                  <span class="time">(02:00 PM)</span>
                </p>
              </div>
 </div></b-card-text>
      </b-tab>
      <b-tab title="On This age">
        <b-card-text>            <div class="messages-box">
              <div class="forword-msg">
                <p>
                  <b-form-checkbox
                    id="checkbox-1"
                    name="checkbox-1"
                    value="accepted"
                    unchecked-value="not_accepted"
                  >
                  </b-form-checkbox>
                  <strong>Vasilii Kovalchuk</strong>
                  <span class="h5">Home Page</span> One morning, when Gregor
                  Samsa woke from troubled dreams, he found himself transformed
                  <span class="time">(02:00 PM)</span>
                </p>
              </div>
              <div class="forword-msg">
                <p>
                  <b-form-checkbox
                    id="checkbox-2"
                    name="checkbox-3"
                    value="accepted"
                    unchecked-value="not_accepted"
                  >
                  </b-form-checkbox>
                  <strong>Vasilii Kovalchuk</strong>
                  <span class="h5">Team Page</span>"What's happened to me?" he
                  thought. It wasn't a dream. His room, a proper human room
                  although a little
                  <span class="time">(02:00 PM)</span>
                </p>
              </div>
              <div class="forword-msg">
                <p>
                  <b-form-checkbox
                    id="checkbox-3"
                    name="checkbox-3"
                    value="accepted"
                    unchecked-value="not_accepted"
                  >
                  </b-form-checkbox>
                  <strong>Vasilii Kovalchuk</strong>
                  <span class="h5">Team Page</span>A collection of textile
                  samples lay spread out on the table
                  <span class="time">(02:00 PM)</span>
                </p>
              </div>
 </div></b-card-text>
      </b-tab>
    </b-tabs>
  </b-card>
</div>
      <div class="flex-msg-box2 h-100">
        <div class="enter-message">
          <b-form>
            <b-form-input
              id="inline-form-input-name"
              placeholder="Enter Message ..."
            ></b-form-input>
            <div class="send-box">
              <b-button variant="primary" class="send">
                Create
              </b-button>
            </div>
          </b-form>
        </div>
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
.groupchat-sidebar .forword-msg p span.h5 {
  font-weight: 500;
  font-size: 14px;
  display: block;
}
.nots-tabs .forword-msg p span.time {
  right: auto;
  bottom: auto;
  top: 11px;
  left: 105px;
}
.nots-tabs .nav-tabs {
  background: #f9f9f9;
}
.nots-tabs .nav-tabs .nav-link {
  font-weight: 500;
  font-size: 14px;
}
.nots-tabs .nav-tabs .nav-link.active,
.nots-tabs .nav-tabs .nav-item.show .nav-link {
  background-color: transparent;
  border-color: transparent;
  color: #4489fe;
  border-bottom: 3px solid #4489fe;
}
.nots-tabs .nav-tabs .nav-link {
  font-weight: 500;
  font-size: 14px;
  color: #212121;
  padding: 16px 0;
}
.nots-tabs li.nav-item {
  width: 50%;
  text-align: center;
}
.nots-tabs .forword-msg p:last-child:after {
  display: none;
}
.nots-tabs .nav-tabs .nav-link:hover {
  border-color: transparent;
  color: #4489fe;
  border-bottom: 3px solid #4489fe;
}
.nots-tabs .messages-box {
  max-height: 300px;
}
.nots-tabs .custom-control {
  position: absolute;
  right: 8px;
  top: 9px;
}
.nots-tabs .custom-control-label::before,
.nots-tabs .custom-control-label::after {
  width: 24px;
  height: 24px;
  border-radius: 100% !important;
  cursor: pointer;
}
.nots-tabs .card-header {
    padding: 0 10px;
}
.nots-tabs  .card-body {
    padding: 12px 0 0;
}
.nots-tabs .card {
    border: 0;
}
.groupchat-sidebar .nots-tabs .forword-msg p {
  background: #e9f0fd;
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
