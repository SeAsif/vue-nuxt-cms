<template>
  <div>
    <div class="header">
       <b-container class="p-0">
      <template>
        <div class="sidebar-box">
           <b-navbar-brand class="menu-icon" v-b-toggle.sidebar-1>
             <b-img src="~assets/i/menu-icon.svg"
          />
          </b-navbar-brand>
          <b-navbar-brand to="/" >
            <NuxtLink to="/" class="d-flex logoMain">
              <b-img class="logo" src="~assets/i/logo.svg" height="40" />
              <h2 class="logoText mb-0">CMS</h2>
            </NuxtLink>
          </b-navbar-brand>
        </div>
        <b-sidebar id="sidebar-1" title="Sidebar" shadow>
          <div class="px-3 py-2">
            <p>
              Cras mattis consectetur purus sit amet fermentum. Cras justo odio,
              dapibus ac facilisis in, egestas eget quam. Morbi leo risus, porta
              ac consectetur ac, vestibulum at eros.
            </p>
            <b-img
              src="https://picsum.photos/500/500/?image=54"
              fluid
              thumbnail
            ></b-img>
          </div>
        </b-sidebar>
      </template>
      <b-navbar type="light" variant="faded">
        <div class="tesktop-nav"></div>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <div class="last-sixli">
            <b-nav-form>
              <b-form-input
                size="sm"
                class="mr-sm-2"
                placeholder="Search DeskVantage"
              ></b-form-input>
              <b-button size="sm" class="my-2 my-sm-0" type="submit"
                ><b-img src="~assets/i/search-btn.svg"
              /></b-button>
            </b-nav-form>

            <b-nav-item href="#">Pages</b-nav-item>
            <b-nav-item to="general-setting">Directory</b-nav-item>

            <b-nav-item-dropdown class="change-color-a" text="Content" right>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
            </b-nav-item-dropdown>

            <b-nav-item-dropdown class="change-color-a" text="Team" right>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-item-dropdown class="change-color-a" text="Templates" right>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
              <b-dropdown-item href="#">Pages</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-item href="#">Settings</b-nav-item>
            </div>
          </b-navbar-nav>

        </b-collapse>
      </b-navbar>
                          <b-navbar-nav>

            <div class="last-threeli">
            <b-nav-item href="#" class="msg-box dote mr-20"
              ><b-img src="~assets/i/chat.svg"
            /></b-nav-item>
            <b-nav-item href="#" class="msg-box dote"
              ><b-img src="~assets/i/document.svg"
            /></b-nav-item>
            <b-nav-item href="#" class="user-box"
              ><b-img class="userImg" src="~assets/i/user.svg"
            /></b-nav-item>
            </div>
          </b-navbar-nav>
      </b-container>
      </div>

  </div>
</template>

<style scoped>
.logoMain:hover{
    text-decoration: none;
  }
.text {
  text-align: center;
}
.nav-desktop {
  width: 130px !important;
  display: flex;
  flex-direction: row-reverse;
  align-items: baseline;
}
.nav-desktop a img {
  width: 50px;
}
.nav-desktop.navbar-dark .navbar-toggler {
  color: #000;
  border-color: transparent;
  padding: 0;
}
.nav-desktop.navbar-dark .navbar-brand {
  margin: 0;
}
.nav-desktop div#nav-collapse {
  position: absolute;
  left: 19px;
  top: 50px;
  z-index: 9;
}
.header {
    display: flex;
    width: 100%;
    border-bottom: 1px solid #e5e9ee;
    position: fixed;
    z-index: 9;
    top: 0;
    background-color: #fff;
    padding-left: 20px;
}
.header .container {
  display: flex;
  width: 100%;
  justify-content: space-between;
  margin: 0;
  max-width: 100% !important;

}
.header button.btn.btn-secondary.collapsed {
  background: no-repeat;
  border: none;
}
.header button.btn.btn-secondary.collapsed img {
  width: 26px;
}
.sidebar-box {
  display: flex;
  align-items: center;
  width: 131px;
  justify-content: space-between;
}

.header .btn {
  transition: auto;
}
.header .navbar-dark .navbar-nav .nav-link {
  color: #212121 !important;
}
li.form-inline button.btn {
  position: absolute;
  left: 13px;
  top: 9px;
  background: none;
  border: none;
}
li.form-inline {
  position: relative;
}
li.form-inline input {
  height: 50px;
  width: 240px;
  background-color: #f2f3f5;
  padding: 0 10px 0 53px;
  border-radius: 8px;
  border: none;
}
 .navbar-nav {
  display: flex;
  align-items: center;
  justify-content: center;
}
.header li.nav-item.msg-box.dote a img {
  width: 20px;
}

.header li.nav-item.msg-box.dote a {
  width: 50px;
  height: 50px;
  background-color: #e9f0fd;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #212121;
}
.header li.nav-item.user-box {
  width: 40px;
  height: 40px;
  border-radius: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-right: 15px;
}
.userImg {
  width: 40px;
  height: 40px;
}
.mr-20 {
  margin-right: 20px;
}
.header ul li {
  margin-right: 21px;
}
.navbar-light .navbar-nav .nav-link {
  color: #212121;
}
.header .last-threeli {
    display: flex;
    align-items: center;
}
.header .last-sixli {
    display: flex;
    align-items: center;
}
</style>
