<template>
  <div>
    <div class="general-settings-page">
      <h3>Home Page <b-img src="~assets/i/eye-blue.svg" /></h3>
      <b-button block variant="primary" class="text-left general-btn"
        ><b-img src="~assets/i/setting.svg" />General Settings</b-button
      >
  <div class="generals-scroll">
      <div class="levels arrow-selectar">
        <b-button
          :class="visible ? null : 'collapsed'"
          :aria-expanded="visible ? 'true' : 'false'"
          aria-controls="collapse"
          @click="visible = !visible"
        >
          <b-img src="~assets/i/menu-icon-general.svg" />
          <span> Menu Sections</span>
        </b-button>
        <b-collapse id="collapse" v-model="visible">
          <b-list-group-item>
            <b-list-group>
              <b-list-group-item button class="dirlist active" ><NuxtLink to="banner">Banner</NuxtLink> </b-list-group-item>
              <b-list-group-item button class="dirlist">Industries</b-list-group-item>
              <b-list-group-item button class="dirlist">About us</b-list-group-item>
              <b-list-group-item button class="dirlist">New Ideas</b-list-group-item>
              <b-list-group-item button class="dirlist">Blog</b-list-group-item>
              <b-list-group-item button class="dirlist">Contracts</b-list-group-item>
              <b-list-group-item button class="dirlist">Portal</b-list-group-item>
            </b-list-group>
          </b-list-group-item>
        </b-collapse>
      </div>
      <b-button
        class="btn-blue"
        variant="link"
        id="show-btn"
        @click="$bvModal.show('bv-modal-example')"
        >Add Section</b-button
      >
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      visible: true
    };
  }
};
</script>
<style scoped>
.active{
  background: #e9f0fd;
  border-radius: 8px;
  border: 0;
  color: #4489fe;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  padding: 15px 16px;
  display: flex;
  align-items: center;
}
.levels button {
  width: 100%;
  text-align: left;
  background-color: transparent !important;
  font-size: 14px;
  color: #212121;
  border: 0;
  padding: 12px 12px;
}
.levels button:active {
  box-shadow: none;
}
.levels button:focus {
  box-shadow: none;
}
.levels .list-group-item {
  border: 0;
  padding: 4px 0 20px;
}
.general-settings-page {
  border: 1px solid #e5e9ee;
    padding: 22px 15px;
    border-top: 0;
    border-bottom: 0;
    height: calc(100vh - 172px);
    overflow-y: hidden;
    overflow-x: hidden;
}
.general-settings-page h3 {
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 0px 7px 12px;
}
.general-settings-page .btn-primary.general-btn {
  background: #e9f0fd;
  border-radius: 8px;
  border: 0;
  color: #4489fe;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  padding: 15px 14px;
  display: flex;
  align-items: center;
}
.general-settings-page .btn-blue {
  width: 220px;
  height: 44px;
  margin: 19px auto 0;
}
.general-settings-page img {
  margin-right: 17px;
}
.general-settings-page h3 img {
  margin-right: 14px;
}
.general-settings-page .menu-btn {
  background: none;
  border: 0;
  color: #212121;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
}
.general-settings-page .list-group button {
  border: 0;
  color: #212121;
  font-weight: normal;
  font-size: 14px;
  border-radius: 8px;
  padding: 14px 11px;
}
.general-settings-page .list-group button:after {
  position: absolute;
  content: "";
  left: -14px;
  top: 24px;
  width: 20px;
  height: 1px;
  background-repeat: no-repeat;
  pointer-events: none;
  background: #e5e9ee;
}
.general-settings-page .list-group {
  border-left: 1px solid #e5e9ee;
  margin-left: 21px;
  padding-left: 14px;
}
.general-settings-page.arrow-selectar:after {
  top: 15px;
  background-color: transparent !important;
}
.levels .arrow-selectar:after {
  top: 21px;
}
.general-settings-page .list-group button:last-child {
  padding-bottom: 0px;
  line-height: 2px;
  padding-top: 25px;
}
</style>
