<template>
  <div>
    <b-container>
      <div class="text-sites">
        <h2>Sites</h2>
        <b-button
          class="btn-blue"
          variant="link"
          id="show-btn"
          @click="$bvModal.show('bv-modal-example')"
          >Add Site</b-button
        >
      </div>
      <div class="project-flex">
        <div class="project-box one">
          <div class="logo-box"><b-img src="~assets/i/desk-logo.svg" /></div>
          <div class="text-box">
            <div class="pro-box">
              <p>Project</p>
              <p>6 weeks ago</p>
            </div>
            <h3>DeskVantage</h3>
            <ul>
              <li><b-img src="~assets/i/boy.svg" /></li>
              <li class="two"><b-img src="~assets/i/boy.svg" /></li>
              <li class="three"><b-img src="~assets/i/boy.svg" /></li>
              <li class="four"><b-img src="~assets/i/boy.svg" /></li>
              <li class="five"><b-img src="~assets/i/boy.svg" /></li>
              <li class="six"><b-button class="bg-white">6+</b-button></li>
            </ul>
            <b-button to="Settings" block class="btn-grey-outline">Settings</b-button>
          </div>
        </div>
        <div class="project-box">
          <div class="logo-box"><b-img src="~assets/i/just.svg" /></div>
          <div class="text-box">
            <div class="pro-box">
              <p>Project</p>
              <p>6 weeks ago</p>
            </div>
            <h3>Nike Pro</h3>
            <ul>
              <li><b-img src="~assets/i/boy.svg" /></li>
              <li class="two"><b-img src="~assets/i/boy.svg" /></li>
              <li class="three"><b-img src="~assets/i/boy.svg" /></li>
            </ul>
            
            <b-button to="Settings" block class="btn-grey-outline">Settings</b-button>
          </div>
        </div>
      </div>
    </b-container>
  </div>
</template>

<style scoped>
.project-box {
  max-width: 300px;
  width: 100%;
  border: 1px solid #e5e9ee;
  box-sizing: border-box;
  border-radius: 4px;
}
.project-box .logo-box {
  padding: 30px 0;
  max-height: 140px;
  min-height: 140px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-bottom: 1px solid #E9F0FD;
}
.project-box .text-box p {
  font-style: normal;
  font-weight: bold;
  font-size: 10px;
  color: #b4b4b4;
  margin: 0 0 5px;
  text-transform: uppercase;
}
.project-box .text-box .pro-box {
  display: flex;
  justify-content: space-between;
}
.project-box .text-box h3 {
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  color: #212121;
  margin-bottom: 21px;
}
.project-box .text-box {
  background-color: #f8faff;
  padding: 19px 21px;
}
.project-box.one {
  margin-right: 30px;
}
.project-box .text-box ul {
  padding: 0;
  margin: 0;
  margin-bottom: 26px;
}
.project-box .text-box ul {
  display: flex;
  align-items: center;
}
.project-box .text-box ul li {
  list-style-type: none;
  width: 38px;
  height: 38px;
  border-radius: 100%;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  border: 5px solid #fff;
}
.project-box .text-box ul li img {
  width: 100%;
  height: auto;
  display: block;
}
.project-box .text-box ul li button {
  color: #b4b4b4 !important;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
}
.project-box .text-box ul li.two {
  transform: translate(-17px, 0);
}
.project-box .text-box ul li.three {
  transform: translate(-34px, 0);
}
.project-box .text-box ul li.four {
  transform: translate(-51px, 0);
}
.project-box .text-box ul li.five {
  transform: translate(-68px, 0);
}
.project-box .text-box ul li.six {
  transform: translate(-85px, 0);
}
.project-box .text-box a {
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  color: #7d7d7d;
  width: 100%;
  display: block;
  text-align: center;
  border: 1px solid #dee0e4;
  box-sizing: border-box;
  border-radius: 4px;
  padding: 8px 0;
}
.project-flex {
  display: flex;
  margin-bottom: 60px;
}
.text-sites {
  padding: 38px 0 30px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.text-sites button.btn.btn-primary {
  width: 200px;
  height: 44px;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
}
</style>
