<template>
  <div>
    <div class="chat-sidebar">
      <div class="chat-box">
        <h1 class="m-0">All Chats</h1>
        <b-button variant="primary">Create</b-button>
      </div>
      <div class="chat-searchbar">
        <b-nav-form>
          <b-form-input
            size="sm"
            class="mr-sm-2"
            placeholder="Search"
          ></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit"
            ><b-img src="~assets/i/search-btn.svg"
          /></b-button>
        </b-nav-form>
      </div>

      <div class="list-chat">
        <b-list-group>
          <b-list-group-item href="#">
            <div class="img-box">
              <b-img src="~assets/i/chatboy-one.svg" />
            </div>
            <div class="text-box">
              <h4>Artem Reza</h4>
              <p>You: One morning, when Gregor Samsa woke from troubled</p>
              <span class="text-data">
                1/11/2020
              </span>
              <strong class="notification">11</strong>
            </div>
          </b-list-group-item>
          <b-list-group-item href="#">
            <div class="img-box np">
              <strong>NP</strong>
            </div>
            <div class="text-box">
              <h4>New Project Group</h4>
              <p>You: One morning, when Gregor Samsa woke from troubled</p>
              <span class="text-data">
                1/11/2020
              </span>
            </div>
          </b-list-group-item>
          <b-list-group-item href="#">
            <div class="img-box">
              <b-img src="~assets/i/chatboy-two.svg" />
            </div>
            <div class="text-box">
              <h4>Vasilii Kovalchuk</h4>
              <p>You: One morning, when Gregor Samsa woke from troubled</p>
              <span class="text-data">
                1/11/2020
              </span>
            </div>
          </b-list-group-item>
          <b-list-group-item href="#" active>
            <div class="img-box">
              <b-img src="~assets/i/chatboy-three.svg" />
            </div>
            <div class="text-box">
              <h4>Vlad Sklyar</h4>
              <p>You: One morning, when Gregor Samsa woke from troubled</p>
              <span class="text-data">
                1/11/2020
              </span>
            </div>
          </b-list-group-item>
          <b-list-group-item href="#">
            <div class="img-box">
              <b-img src="~assets/i/chatboy-four.svg" />
            </div>
            <div class="text-box">
              <h4>Artem Reza</h4>
              <p>You: One morning, when Gregor Samsa woke from troubled</p>
              <span class="text-data">
                1/11/2020
              </span>
            </div>
          </b-list-group-item>
        </b-list-group>
      </div>
    </div>
  </div>
</template>

<style>
.chat-box {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 26px 0;
}
.chat-box h1 {
  font-weight: normal;
  font-size: 24px;
  color: #212121;
}
.chat-box button {
  width: 66px;
  height: 27px;
  background: #4489fe;
  border-radius: 4px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
}
.chat-searchbar {
  position: relative;
  border-top: 1px solid #e5e9ee;
  border-bottom: 1px solid #e5e9ee;
}
.chat-searchbar input {
  width: 100% !important;
  height: 53px !important;
  border: 0;
  padding-left: 46px;
}
.chat-searchbar input:focus {
  box-shadow: none;
}
.chat-searchbar button {
  background: none;
  border: 0;
  position: absolute;
  left: 8px;
}
.chat-searchbar button:hover {
  background: none;
}
.chat-searchbar button:focus {
  box-shadow: none;
}
.chat-searchbar .btn-secondary.focus {
  background-color: none !important;
}
.chat-searchbar .form-inline {
  width: 100%;
}
.list-chat a.list-group-item {
  display: flex;
  align-items: center;
  padding: 6px 7px 6px 33px;
  justify-content: space-between;
}
.list-chat a.list-group-item .img-box {
  width: 44px;
  height: 44px;
  overflow: hidden;
  border-radius: 100%;
}
.list-chat a.list-group-item .img-box.np {
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #e67cef;
  color: #fff;
}
.list-chat a.list-group-item .text-box h4 {
  font-weight: bold;
  font-size: 13px;
  margin: 0;
}
.list-chat a.list-group-item.active .text-box h4,
.list-chat a.list-group-item.active .text-box p,
.list-chat a.list-group-item.active .text-box span.text-data {
  color: #fff;
}
.list-chat a.list-group-item:hover .text-box h4,
.list-chat a.list-group-item:hover .text-box p,
.list-chat a.list-group-item:hover .text-box span.text-data {
  color: #fff;
}
.list-chat a.list-group-item:hover {
  background-color: #4489fe;
}
.list-chat a.list-group-item:hover .text-box strong.notification {
  background-color: #fff;
  color: #4489fe;
}
.list-chat {
  margin-left: -22px;
}
.list-chat a.list-group-item.active {
  color: #fff;
  background-color: #4489fe;
}
.list-chat a.list-group-item .text-box p {
  font-weight: normal;
  font-size: 12px;
  color: #b4b4b4;
  margin: 6px 0 0;
}
.list-chat a.list-group-item .text-box {
  margin-left: 12px;
  padding-right: 13px;
  width: 216px;
}
.list-chat a.list-group-item .text-box span.text-data {
  font-weight: normal;
  font-size: 11px;
  color: #b4b4b4;
  position: absolute;
  top: 4px;
  right: 11px;
}
.list-chat a.list-group-item .text-box strong.notification {
  width: 20px;
  height: 20px;
  background: #4489fe;
  border-radius: 100%;
  font-weight: normal;
  font-size: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  right: 11px;
  top: 34px;
  color: #fff;
}
.list-chat a.list-group-item.active .text-box:after {
  display: none;
}
.list-chat a.list-group-item .text-box:after {
  content: "";
  width: 228px;
  height: 1px;
  background: #e5e9ee;
  position: absolute;
  right: 0;
  bottom: 0;
}
.list-chat .list-group-item {
  border: 0;
}
</style>
