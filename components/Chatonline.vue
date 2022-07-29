<template>
  <div class="h-100">
    <div class="online-centerbar h-100">
      <div class="online-box">
        <div class="after-dote">
          <div class="img-box">
            <b-img src="~assets/i/chatboy-three.svg" />
          </div>
          <span class="online-dote"></span>
        </div>
        <div class="vlad-text text-center">
          <h5 class="m-0">Vlad Sklyar</h5>
          <span>Online</span>
        </div>
        <div class="search-dropdown">
          <b-button size="sm" class="my-2 my-sm-0" type="submit"
            ><b-img src="~assets/i/search-btn.svg"
          /></b-button>
          <b-dropdown
            id="dropdown-offset"
            offset="25"
            text="..."
            class=" dropdown-box"
          >
            <b-dropdown-item href="#">Action</b-dropdown-item>
            <b-dropdown-item href="#">Another action</b-dropdown-item>
            <b-dropdown-item href="#">Something else here</b-dropdown-item>
          </b-dropdown>
        </div>
      </div>
      <div class="flex-msg-box h-100">
        <div class="messages-box">
          <div class="forword-msg">
            <p>
              Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean
              commodo ligula eget dolor. Aenean massa<span class="time"
                >5:20 PM</span
              >
            </p>
            <p>Hey What’s up man?<span class="time">5:20 PM</span></p>
            <p>
              How u doing? Do u wanna change some bitcoins? Location: Kyiv<span
                class="time"
                >5:20 PM</span
              >
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
              Of course, I have. And do you have money to buy them? =)<span
                class="time"
                >5:20 PM</span
              >
            </p>
          </div>
          <div class="in-msg">
            <p>
              Donec pede justo, fringilla vel, aliquet nec, vulputate eget,
              arcu. In enim justo, rhoncus ut<span class="time">5:20 PM</span>
              <strong>Read</strong>
            </p>
          </div>
          <div class="forword-msg">
            <p>
              tiam rhoncus. Maecenas tempus, tellus eget condimentum rhoncus,
              sem quam semper libero<span class="time">5:20 PM</span>
            </p>
            <p>Nam quam nunc, blan<span class="time">5:20 PM</span></p>
            <p>
              How u doing? Do u wanna change some bitcoins? Location: Kyiv<span
                class="time"
                >5:20 PM</span
              >
            </p>
          </div>
          <div class="in-msg">
            <p>
              Maecenas nec odio et ante tincidunt tempus. Donec vitae sapien ut
              libero venenatis faucibus. <span class="time">5:20 PM</span>
              <strong>Read</strong>
            </p>
          </div>
          <div class="forword-msg">
            <p>
              Duis leo. Sed fringilla mauris sit amet nibh. Donec sodales
              sagittis magna.<span class="time">5:20 PM</span>
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
.online-box .img-box {
  width: 44px;
  height: 44px;
  overflow: hidden;
  border-radius: 100%;
}
span.online-dote {
  width: 9px;
  height: 9px;
  background: #0faa58;
  display: block;
  border-radius: 100%;
  border: 1px solid #fff;
  position: absolute;
  left: 33px;
  top: 34px;
}
.after-dote {
  position: relative;
}
.online-box {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 13px 30px;
  border-bottom: 1px solid #e5e9ee;
  height: 70px;
  background: #fff;
}
.vlad-text h5 {
  font-weight: 500;
  font-size: 15px;
}
.vlad-text span {
  font-weight: 500;
  font-size: 13px;
  color: #0faa58;
}
.search-dropdown .dropdown-box button.btn.btn-secondary {
  background: none;
  border: none;
  font-size: 25px;
  color: #969696;
  transform: translate(6px, -4px);
}
.online-centerbar {
  border: 1px solid #f9f9f9;
  background: #f9f9f9;
}
</style>
