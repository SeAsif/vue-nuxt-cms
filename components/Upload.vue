<template>
  <div>
    <div class="tab-1">
  
      <div class="information-box">
      
        <div class="d-block text-center">
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
.information-box {
    padding:0 !important;}
    .upload-file {
    margin: 20px 0 0px 0 !important;}
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
 
  border-radius: 4px;
}
</style>
