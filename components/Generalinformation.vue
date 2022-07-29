<template>
  <div>
    <div class="tab-1">
      <div class="back-btn">
        <b-button class="back-btn">
          <b-img src="~assets/i/back-btn.svg" /> Back</b-button
        >
      </div>
      <div class="information-box pt-4 scroll-general">
        <h4>General Information</h4>
        <div class="d-block text-center">
          <b-form>
            <b-row>
              <b-col cols="6">
                <div class="input-box">
                  <label for="input-with-list">Site Name</label>
                  <b-form-input
                    placeholder="Nike Pro"
                  ></b-form-input>
                </div>
              </b-col>
              <b-col cols="6">
                <div class="input-box">
                  <label for="input-with-list">URL</label>
                  <b-form-input
                    placeholder="www.nilepro.com"
                  ></b-form-input>
                </div>
              </b-col>
            </b-row>
          </b-form>
          <div class="upload-file">
            <b-img src="~assets/i/drag.svg" />
            <h4>Drag and drop your site logo here</h4>
            <div class="upload-btn">
              <p>Upload</p>
              <b-form-file v-model="file2" class="mt-3" plain></b-form-file>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.back-btn button.back-btn {
  background: none;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  color: #757575;
  border: none;
  padding: 0;
}
.back-btn {
  min-height: 33px;
}
.input-box {
  text-align: left;
}
.input-box label {
  color: #7d7d7d;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  margin: 0;
  background-color: #fff;
  transform: translate(14px, 11px);
  padding: 0 5px;
}
.input-box input {
  border: 1px solid #e5e9ee;
  border-radius: 4px;
  height: 50px !important;
  padding: 0 18px !important;
}
.upload-file {
  text-align: center;
  background: #e9f0fd;
  border: 1px dashed #d8d8d8;
  border-radius: 4px;
  padding: 53px 15px;
  margin: 30px 0 14px;
}
.upload-file h4 {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  color: #212121;
  margin: 13px 0;
}
.upload-btn {
  width: 125px;
  height: 34px;
  display: flex;
  align-items: center;
  cursor: pointer;
  background-color: #4489fe;
  border-radius: 3px;
  position: relative;
  text-align: center;
  justify-content: center;
  margin: 0 auto;
  transition: all 0.6s;
}
.upload-btn[data-v-3598487d] {
  opacity: 0.9;
}

.upload-btn input {
  position: absolute;
  top: -16px;
  margin: 0;
  height: 34px;
  opacity: 0;
  cursor: pointer;
}
.upload-btn p {
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  margin: 0;
  color: #ffffff;
}
.information-box h4 {
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  color: #212121;
}
.information-box {
  border: 0.5px solid #dadce0;
  border-radius: 4px;

}
.scroll-general{
  /* max-height: calc(100vh - 182px);
    overflow-y: scroll;
    overflow-x: hidden;
    scroll-behavior: smooth; */
}
.scroll-general::-webkit-scrollbar-track
{
	-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
	background-color: #F5F5F5;
}

.scroll-general::-webkit-scrollbar
{
	width: 6px;
	background-color: #F5F5F5;
}

.scroll-general::-webkit-scrollbar-thumb
{
	background-color: #000000;
}



</style>
