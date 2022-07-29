<template>
  <div>
    <Nuxt />
  </div>
</template>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

/*
 *  STYLE 3
 */

#scrollStyle3{
  /* scrollbar-width: thin;
  scrollbar-color: #e3e3e3 transparent;
      overflow-y: scroll;
    max-height: 100vh; */
}
#scrollStyle3::-webkit-scrollbar-track
{
	-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
	background-color: #F5F5F5;
}

#scrollStyle3::-webkit-scrollbar
{
	width: 6px;
	background-color: #F5F5F5;
}

#scrollStyle3::-webkit-scrollbar-thumb
{
	background-color: #000000;
}

body {
    min-width: 1200px;
    /* overflow-x: scroll !important; */
    scrollbar-width: thin;
  scrollbar-color: #e3e3e3 transparent;
    overflow-y: scroll;
}

body::-webkit-scrollbar {
  width: 5px;
}

body::-webkit-scrollbar-track {
  box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
  border-radius: 10px;
  background: transparent;
}

body::-webkit-scrollbar-thumb {
  background-color: darkgrey;
  outline: 1px solid slategrey;
}
/* #scrollStyle3{
    height: 100vh;
    overflow-x: hidden;
    overflow-y: scroll;
    margin-top: -67px;
    padding-top: 67px;} */

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  color: #212121;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}
.change-color-a a::after {
  display: none;
}
.change-color-a a {
  position: relative;
  padding-right: 24px !important;
}
.change-color-a .dropdown-menu a::before {
  display: none;
}
.change-color-a .dropdown-menu li {
  margin-right: 0 !important;
}
.change-color-a a::before {
  position: absolute;
  content: "";
  right: 2px;
  top: 17px;
  background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTEiIGhlaWdodD0iNiIgdmlld0JveD0iMCAwIDExIDYiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxwYXRoIGQ9Ik0xMC45MTEgMC45MDE4ODlDMTAuOTExIDEuMTMxNzYgMTAuODIzMiAxLjM2Mjg0IDEwLjY0NzQgMS41Mzg1NUw2LjQ3MTIzIDUuNzM1MjNDNi4zMDE1NCA1LjkwNDkyIDYuMDcxNjYgNiA1LjgzMDk2IDZDNS41OTE0NiA2IDUuMzYxNTkgNS45MDQ5MiA1LjE5MTg5IDUuNzM1MjNMMS4wMTMyNyAxLjUzODU1QzAuNjYxODQzIDEuMTg1OTIgMC42NjE4NDMgMC42MTU0NTIgMS4wMTU2OCAwLjI2MjgyQzEuMzY5NTEgLTAuMDg4NjA3NCAxLjk0MTE4IC0wLjA4NzQwMzkgMi4yOTI2MSAwLjI2NTIyN0w1LjgzMDk2IDMuODE5MjJMOS4zNjkzMSAwLjI2NTIyN0M5LjcyMDc0IC0wLjA4NzQwMzkgMTAuMjkxMiAtMC4wODg2MDc0IDEwLjY0NSAwLjI2MjgyQzEwLjgyMzIgMC40Mzg1MzQgMTAuOTExIDAuNjcwODE0IDEwLjkxMSAwLjkwMTg4OVoiIGZpbGw9IiMyMDBFMzIiLz4KPC9zdmc+Cg==);
  z-index: 999;
  width: 12px;
  height: 8px;
  background-repeat: no-repeat;
  pointer-events: none;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}
/* .hover-switch img.two {
  left: 14px;
  top: 24px;
}
.hover-switch img.one {
  left: 15px !important;
  top: 24px !important;
} */

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
.arrow-selectar {
  position: relative;
}
.arrow-selectar:after {
  position: absolute;
  content: "";
  right: 27px;
  top: 48px;
  background-image: url("~assets/i/arrow-selectar.svg");
  z-index: 999;
  width: 20px;
  height: 20px;
  background-repeat: no-repeat;
  pointer-events: none;
  background-color: #fff;
}
.eys-after {
  position: relative;
}
.eys-after:before {
  position: absolute;
  content: "";
  right: -34px;
  top: 43px;
  background-image: url(/_nuxt/assets/i/eys.svg);
  z-index: 999;
  width: 20px;
  height: 20px;
  background-repeat: no-repeat;
}
.sidebar-main h3 {
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  color: #757575;
  margin-bottom: 27px;
}
.sidebar-main {
  margin: 0;
  padding: 0;
}
.sidebar-main li .text h4 {
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  color: #212121;
  margin: 0;
}
.sidebar-main li .text p {
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  color: #757575;
  margin: 0;
}
.sidebar-main li {
  list-style: none;
}
.setting-sidebar li a {
  display: flex;
  align-items: center;
  border: 0.5px solid #dadce0 !important;
  border-radius: 4px;
  padding: 15px 29px;
  text-decoration: none;
  position: relative;
  transition: all 0.6s;
  margin-block: 6px;
  width: 100%;
}
.setting-sidebar {
    margin-top: -27px;
    /* position: sticky; */
    top: 25px;
}
.sidebar-main li a:hover {
  border-left: 5px solid #4489fe !important;
  background: #f3f7ff;
}
.sidebar-main div#dropdown-offset li a:hover {
  border-left: 0 !important;
}


.sidebar-main li a.active img:first-of-type {
    opacity: 0;
}
.sidebar-main li a.active img:last-of-type {
    opacity: 1;
}

.sidebar-main li a.active {
  display: flex;
  align-items: center;
  border-left: 5px solid #4489fe !important;
  background: #f3f7ff !important;
  width: 100%;
}

.sidebar-main {
  margin-top: 3px;
}
.sidebar-main li a .text {
  margin-left: 22px;
}
.hover-switch img {
  position: absolute;
  top: calc(50% - 100px);
  left: calc(50% - 100px);
  left: 16px;
  top: 25px;
  width: 18px;
  height: 18px;
}
.hover-switch:hover img {
  opacity: 0;
}
.sidebar-box .btn-secondary:focus {
  box-shadow: 0 0 0 0.2rem rgb(130 138 145 / 0%) !important;
}
.project-box .btn-secondary:hover {
  background-color: transparent;
}
.hover-switch img:last-of-type {
  opacity: 0;
}
.btn-blue:hover {
  color: #7d7d7d;
  background: none !important;
  border: 1px solid #dee0e4;
  text-decoration: none;
}
.btn-blue:focus {
  /* color: #fff;
  background-color: #4489fe; */
}
.groupchat-sidebar .btn-primary:not(:disabled):not(.disabled):active,
.groupchat-sidebar .btn-primary:not(:disabled):not(.disabled).active {
  background-color: transparent !important;
  color: #212121;
  border: 1px solid #212121;
}
.groupchat-sidebar button:focus {
  color: #212121;
  border: 1px solid #212121 !important;
}
.btn-primary:focus,
.btn-primary.focus {
  background-color: #4489fe !important;
}
.hover-switch:hover img:last-of-type {
  opacity: 1;
}
.sidebar-main .col-auto {
  padding: 0;
  width: 300px;
}
.setting-h3 {
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  color: #757575;
  width: 200px;
  transform: translate(0px, 18px);
}
.general-settings-page .arrow-selectar:after {
  top: 15px;
  right: 10px;
}
.dropdown-box > button {
  background: none;
  color: #212121;
  border: 0;
  padding: 0;
}

.dropdown-box > button:hover {
  color: #212121;
  background-color: transparent !important;
}
.dropdown-box > button:focus {
  color: #212121;
  background-color: transparent !important;
  box-shadow: 0 0 0 0.2rem rgb(130 138 145 / 0%) !important;
}
.btn-secondary:not(:disabled):not(.disabled):active,
.btn-secondary:not(:disabled):not(.disabled).active,
.show > .btn-secondary.dropdown-toggle {
  color: #212121;
  background-color: transparent !important;
}
.dropdown-box > button.dropdown-toggle::after {
  display: none;
}
.main-message .heading {
  background: #e9f0fd;
  border: 1px solid #e5e9ee;
  border-radius: 4px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 12px 30px;
}
.padding-box {
  border: 1px solid #e5e9ee;
  border-radius: 4px;
  padding: 40px 30px 40px;
}
 .input::-webkit-input-placeholder {
  color: #7d7d7da8 !important;
}

 input:-ms-input-placeholder {
  color: #7d7d7da8 !important;
}

 input::placeholder {
  color: #7d7d7da8 !important;
}
 textarea::-webkit-input-placeholder {
  color: #7d7d7da8 !important;
}

 textarea:-ms-input-placeholder {
  color: #7d7d7da8 !important;
}
.search-bar-two.col-lg-3 {
  width: 170px;
  max-width: 22.3%;
}
textarea::placeholder {
  color: #212121;
}
.main-message {
  margin-bottom: 20px;
}
.imgborder-box {
  border: 1px solid #e5e9ee;
  border-radius: 4px;
  min-height: 132px;
}
.blog-checkbox input {
  width: 100%;
  height: 30px;
  cursor: pointer;
}
.input-box input,
.input-box textarea {
  font-size: 14px;
}
.blog-checkbox .custom-control {
  z-index: auto;
}
.blog-checkbox .custom-control-label::before {
  top: 5px;
}
.blog-checkbox .custom-control-label::after {
  top: 5px;
}
.text-flex {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.text-flex .custom-control-label::before {
  width: 36px !important;
  height: 23px;
  border-radius: 50px !important;
  background: #dee0e4;
}
.text-flex .custom-switch .custom-control-label::after {
  width: 19px;
  height: 19px;
  border-radius: 100%;
  background-color: #fff;
}
.arror-color.arrow-selectar:after {
  background-color: transparent;
}
.flex-btn {
  display: flex;
  align-items: center;
  justify-content: center;
}
.flex-btn button.create {
  transition: all 0.6s;
}

.flex-btn button {
  height: 44px;
  width: 200px;
}
.flex-btn button:first-child {
  margin-right: 20px;
}
.flex-btn button.cancel {
  color: #7d7d7d;
  background: none;
  border: 1px solid #dee0e4;
  transition: all 0.6s;
}
.flex-btn button.cancel:hover {
  color: #fff;
  background-color: #007bff;
  border-color: #007bff;
}
.checkbox {
  margin: 10px 0 5px;
}
.flex-end {
  justify-content: flex-end;
}
.nikepro-icon input {
  padding-left: 45px !important;
}
.nikepro-icon {
  position: relative;
}
.nikepro-icon.arrow-selectar:before {
  position: absolute;
  content: "";
  left: 19px;
  top: 39px;
  background-image: url("~assets/i/nikepro-img.svg");
  z-index: 999;
  width: 20px;
  height: 20px;
  background-repeat: no-repeat;
  pointer-events: none;
  background-color: #fff;
}
.quantity-box label {
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  color: #7d7d7d;
  margin-top: 11px;
}
.quantity-box {
  width: 118px;
  margin-bottom: 7px;
}
.quantity-box button {
  background: #4489fe;
  width: 20px;
  height: 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 5px !important;
}
.quantity-box svg {
  fill: aliceblue;
  width: 16px;
}
.quantity-box output#sb-input {
  border: 1px solid #e5e9ee;
  border-radius: 4px;
  margin: 0 15px;
  height: 44px;
  display: flex;
  align-items: center;
}
.quantity-box .form-control {
  overflow: inherit;
  display: flex !important;
  align-items: center !important;
  justify-content: center;
  border: 0;
  outline: none;
}
.quantity-box .form-control:focus {
  box-shadow: 0 0 0 0.2rem rgb(0 123 255 / 0%) !important;
}
.quantity-box .form-control.focus {
  box-shadow: 0 0 0 0.2rem rgb(0 123 255 / 0%) !important;
}
span.last.text-flex button {
  background: none;
  border: 0;
  padding: 0;
}
span.last.text-flex .custom-switch {
  margin: 0 17px;
}
.chat-box {
  height: 70px;
}

.messages-box {
  padding: 11px 75px 40px 75px;
  background: #f9f9f9;
  max-height: 348px;
  overflow-y: scroll;
  position: relative;
}
.messages-box::-webkit-scrollbar {
  display: none;
}
.forword-msg p {
  background: #ffffff;
  border-radius: 15px;
  padding: 12px 30px 18px 13px;
  font-weight: normal;
  font-size: 13px;
  color: #212121;
  position: relative;
  max-width: 490px;
  display: inline-block;
  margin-bottom: 6px;
}
.forword-msg p span.time {
  font-weight: normal;
  font-size: 12px;
  color: #b4b4b4;
  position: absolute;
  right: 15px;
  bottom: 0;
}
.forword-msg p:last-child:after {
  content: "";
  background-image: url("~assets/i/forword-arrow.svg");
  background-repeat: no-repeat;
  position: absolute;
  left: -6px;
  bottom: -6px;
  width: 20px;
  height: 20px;
}

.forword-msg {
  position: relative;
}
.forword-msg:after {
  content: "";
  background-image: url(/_nuxt/assets/i/chatboy-one.svg);
  background-repeat: no-repeat;
  position: absolute;
  left: -59px;
  bottom: 3px;
  width: 44px;
  height: 44px;
}

.in-msg p {
  background: #4489fe;
  border-radius: 15px;
  padding: 12px 30px 18px 13px;
  font-weight: normal;
  font-size: 13px;
  color: #fff;
  position: relative;
  max-width: 490px;
  display: inline-block;
  margin-bottom: 32px;
}
.in-msg p span.time {
  font-weight: normal;
  font-size: 12px;
  color: #fff;
  position: absolute;
  right: 15px;
  bottom: 0;
}
.in-msg p:last-child:after {
  content: "";
  background-image: url("~assets/i/in-arrow.svg");
  background-repeat: no-repeat;
  position: absolute;
  right: -13px;
  bottom: -6px;
  width: 20px;
  height: 20px;
}
.in-msg {
  position: relative;
  display: flex;
  justify-content: flex-end;
  flex-direction: column;
}
.in-msg:after {
  content: "";
  background-image: url(/_nuxt/assets/i/chatboy-two.svg);
  background-repeat: no-repeat;
  position: absolute;
  right: -59px;
  bottom: 31px;
  width: 44px;
  height: 44px;
}
.in-msg p strong {
  font-weight: normal;
  font-size: 11px;
  color: #7d7d7d;
  position: absolute;
  right: 16px;
  bottom: -20px;
}
.enter-message {
  background: #ffffff;
  border: 1px solid #e5e9ee;
  border-radius: 8px;
  padding: 7px 14px 14px 0;
  margin: 0 15px 31px;
}
.enter-message input {
  font-weight: normal;
  font-size: 13px;
  color: #7d7d7d;
  height: 50px;
  border: 0;
}
.enter-message .send-box {
  display: flex;
  justify-content: flex-end;
}
.enter-message .send-box button {
  background: none;
  border: 0;
  padding: 0 0;
  margin-left: 15px;
}
.enter-message .send-box button.send {
  background: #4489fe;
  border-radius: 4px;
  width: 56px;
  height: 27px;
  font-weight: 500;
  font-size: 14px;
}
.enter-message .form-control:focus {
  box-shadow: none;
}
.messages-box {
  max-height: 275px;
}
.flex-msg-box2 {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.groupchat-sidebar {
  height: 100% !important;
  max-height: 430px;
}
.groupchat-sidebar .messages-box {
  background: transparent;
}
.groupchat-sidebar .messages-box {
  padding: 11px 15px 40px 75px;
}
.groupchat-sidebar .forword-msg p {
  background: #f9f9f9;
}
.groupchat-sidebar .forword-msg p strong {
  font-weight: 500;
  font-size: 11px;
  display: block;
  color: #4489fe;
  margin-bottom: 3px;
}
.flex-msg-box {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.user-box .img img {
  height: 40px;
}
.nots-tabs .forword-msg:after {
  display: none;
}
.groupchat-sidebar .nots-tabs .messages-box {
  padding: 11px 15px 20px 15px;
}

.flex-btn button.create {
  transition: all 0.6s;
}
.flex-btn button {
  height: 44px;
  width: 100%;
}
.flex-btn button.cancel {
  color: #7d7d7d;
  background: none;
  border: 1px solid #dee0e4 !important;
  transition: all 0.6s;
}
.flex-btn button.cancel:hover {
  color: #fff;
  background-color: #007bff;
  border-color: #007bff;
}
.blog-checkbox .custom-checkbox .custom-control-label::before {
  top: 7px;
}
.information-box .upload-file {
  padding: 83px 15px !important;
}
.blog-checkbox .custom-checkbox .custom-control-label::after {
  top: 7px;
}
.blog-checkbox input {
  width: 100%;
  height: 30px;
  cursor: pointer;
}
.vigets-list h4 {
  margin: 0;
}
.scroll-sidebar {
    height: calc(100vh - 240px);
    overflow-y: scroll;
    overflow-x: hidden;
}
.scroll-sidebar::-webkit-scrollbar {
    display: none;
}
.generals-scroll {
  height: calc(100vh - 272px);
    overflow-y: scroll;
    overflow-x: hidden;
    padding-bottom: 20px;
}
.generals-scroll::-webkit-scrollbar {
    display: none;
}
.general-setting{
    height: calc(100vh - 183px);
    overflow-y: scroll;
    overflow-x: hidden;
}
.general-setting::-webkit-scrollbar {
    display: none;
}
.scroll-table{
     /* height: calc(100vh - 200px); */
    overflow-y: scroll;
    overflow-x: hidden;
}
 .scroll-table::-webkit-scrollbar {
    display: none;
}
 .information-box-scroll{
      height: calc(100vh - 124px);
    overflow-y: scroll;
    overflow-x: hidden;
    margin-bottom: 0 !important;
 }
  .information-box-scroll::-webkit-scrollbar {
    display: unset;
}



/* Buttons style here */
button.btn.btn-secondary {
  background: none;
  border: none;
}
button.btn.btn-secondary:focus {
  box-shadow: 0 0 0 0.2rem rgb(130 138 145 / 0%) !important;
}
.btn-grey-outline {
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
  background-color: transparent;
}

.btn-blue {
  font-weight: 500;
  font-size: 14px;
  background-color: #4489fe;
  width: 200px;
  color: white;
  height: 44px;
  border: 1px solid #4489fe;
}
button.dirlist.active{
  background: #e9f0fd;
    border-radius: 8px;
    color: #4489fe;
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
}
/* Buttons style here */


.navbar {
    padding-right: 0;
}
.sidebar-box button {
    padding-left: 17px;
}
span.last ul.dropdown-menu.show {
    transform: translate3d(-164px, 24px, 0px) !important;
}
.text-sites h2 {
    font-size: 24px;
    margin: 0;
}
.tab-content {
    padding-right: 0;
}

.container-100 .container {
    max-width: 100% !important;
}
body{
  padding-top: 67px;
}
.user-box ul.head {
    /* position: sticky; */
    top: 195px;
    background: #fff;
    z-index: 1;
}
.activity-main .user-box ul.head.main {
    top: 67px;
}
.setting-sidebar li:nth-child(1) a {
    padding: 0;
    border: 0 !important;
    pointer-events: none;
}
#input-with-list {
  background-image: url(assets/i/select-arrow.svg);
  height: 50px;
  line-height: 28px;
  background-repeat: no-repeat;
  background-position: 91% 54%;
  cursor: pointer;
  font-size: 14px;
    font-weight: 400;
}
select::-ms-expand {	display: none; }
select{
    -webkit-appearance: none;
    appearance: none;
}
.transcription-services .list-group {
    flex-wrap: wrap;
}
img.logo {
    width: 32px;
    margin-right: 15px;
}
.btn:focus, .btn.focus {
     box-shadow: 0 0 0 0rem rgb(0 123 255 / 0%) !important;
     border: 1px solid #dee0e4;
     text-decoration: none;
}
.header button.btn.btn-secondary.collapsed a {
    display: block;
}
.scroll-general .user-box ul.head {
    top: 43px;
}
.container {
    max-width: 1290px !important;
}
.modal-open {
    overflow: inherit;
}
.flex-btn button {
    font-size: 14px;
}
a.nike-img img {
    width: 20px !important;
    height: auto !important;
}
.levels button img:nth-child(2) {
    width: 24px;
    height: auto;
}
.levels.arrow-selectar:after {
    top: 21px !important;
}
.general-btn.btn-primary:focus, .btn-primary.focus {
    background-color:#e9f0fd !important;
}
.sort-box button {
    border: 1px solid transparent !important;
}
.sort-box button:focus {
    border: 1px solid #000 !important;
}
.levels button.collapsed img:nth-child(1) {
    transform: rotate(
-182deg);
    position: absolute;
    position: absolute;
    left: 0;
    padding: 18px;
}
.levels button.btn-secondary img:nth-child(1) {
    position: absolute;
    left: 0;
    padding: 18px;
}
.generals-scroll .levels button.btn-secondary img:nth-child(1) {
    position: static;
    padding: 0;
}
.general-settings-page .list-group button:hover {
    color: #4489fe !important;
}
.general-settings-page .list-group button a {
        color: #212121;
}
.general-settings-page .list-group button a:hover {
    color: #4489fe !important;
}

.general-settings-page .levels button.collapsed img:nth-child(1) {
    transform: rotate( 
0deg);
}
.box-white{
  position: relative;
}
.box-white:after {
   position: absolute;
    content: "";
    right: 41px;
    top: 10px;
    z-index: 999;
    width: 30px;
    height: 30px;
    background-color: #fff;
    pointer-events: none;
}
.input-box.eys-btn {
    position: relative;
}
.input-box.eys-btn button {
    position: absolute;
    top: 29px;
    right: -50px;
}





@media screen and (max-width: 1360px) {
.header ul li {
    margin-right: 9px !important;
}
.sidebar-box {
    margin-right: 40px;
}

}



@media screen and (max-width: 1200px) {

  .container {
    min-width: 1200px;
    overflow-x: hidden !important;
}
.header {
    position: inherit;
}


.leveltwo .list-group-item {
    padding: 13px 0 13px 0px !important;
}
.header ul li {
    margin-right: 6px !important;
}
li.form-inline input {
    width: 200px !important;
}
.change-color-a a::before {
    top: 16px;
}
.transcription-services .list-group-item {
    margin: 0 0px !important;
}
.navbar-expand-lg .navbar-nav[data-v-1a9bb128] {
    padding-right: 0px !important;
}
}

@media screen and (max-width: 1024px) {
.nikepronav .col-lg-7 {
    padding: 0;
}
.general-settings-page .btn-blue {
    width: 100% !important;
}

}

@media screen and (max-width: 992px) {
.header {
    align-items: baseline;
    position: fixed;
    z-index: 9;
    background: #fff;
    top: 0;
}
.navbar-expand-lg .navbar-nav {
    margin-left: 0!important;
    position: fixed;
    z-index: 9;
    background: #fff;
    left: 0;
    flex-direction: inherit;
     margin: 8px 0 0 0 !important;
}
.header ul li {
    margin-bottom: 5px;
}
.navbar-nav .dropdown-menu {
    position: absolute;
    left: 0;
}
.information-box {
    padding: 22px 15px !important;
}
.user-box ul[data-v-f812c09a] {
    padding: 0 10px !important;
}
.sidebar-main {
    flex-wrap: inherit !important;
}
.pagination {
    padding: 15px 0 20px !important;
}
.margin-0{
  margin: 0 !important;
}
.information-box {
    height: calc(100% - 100px);
}

}


@media screen and (max-width: 768px) {


.container, .container-sm {
    max-width: 100% !important;
}
li.form-inline button.btn {
    margin: 0 !important;
}

}


.pagination {
  justify-content: center;
  padding: 58px 0 30px !important;
  align-items: center;
  border: none !important;
}
.pagination li button,
.pagination li span {
  padding: 6px 11px;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  color: #212121;
  border: none !important;
  border-radius: 4px;
  margin: 0 3px;
}
.pagination li span {
  font-size: 22px !important;
}
[aria-label="Go to next page"],
[aria-label="Go to previous page"]{
  font-size: 22px !important;
}
.pagination_active{
  border-left: 0px solid #4489fe !important;
}
ul.pagination li button:hover {
  border-left: none !important;
  background-color: transparent;
}
.pagination li button.active {
  background-color: #4489fe !important;
  border-radius: 4px;
  color: #fff;
}
.logoText{
    font-size: 22px;
    font-weight: 400;
    display: flex;
    align-items: center;
}
.form-control:focus {
    box-shadow: none !important;
}

</style>













