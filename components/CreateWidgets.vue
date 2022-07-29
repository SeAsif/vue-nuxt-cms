<template>
  <div>
    <div class="tab-1">
      <div class="back-btn">
        <b-button class="back-btn pb-2 d-flex align-items-center">
          <b-img src="~assets/i/back-btn.svg" /> <span class="pl-2">Back</span></b-button
        >
      </div>
      <div class="information-box scroll-general">
        <h4 class="pt-4">General Information</h4>
        <div class="d-block text-center">
          <b-form>
            <b-row>
              <b-col cols="6">
                <div class="input-box">
                  <label for="input-with-list">Widget Name</label>
                  <b-form-input
                    placeholder="Blog"
                  ></b-form-input>
                </div>
              </b-col>
            </b-row>
            <h4 class="text-left mt-4">Widget Template Builder</h4>
            <b-row>
              <b-col cols="6">
                <div class="input-box arrow-selectar">
                  <label for="input-with-list">Select Element</label>
                      <b-form-input
              list="input-list"
              placeholder="Slider"
              id="input-with-list"
            ></b-form-input>
            <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
                </div>
              </b-col>
            </b-row>
            <b-row>
              <b-col cols="6" class="submit-btn">
                <b-button variant="primary" class="btn-blue blue-btn"
                  >Add Element to Widget</b-button
                >
              </b-col>
            </b-row>
          </b-form>
          <Createvidjettable />
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.elHeading{
  font-family: Roboto;
font-style: normal;
font-weight: normal;
font-size: 18px;
line-height: 21px;
color: #212121;
}
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

.submit-btn .blue-btn {
  width: 100%;
  margin-top: 20px;
}
</style>
<script>
export default {
  data() {
    return {
      options: ["Apple", "Banana", "Grape", "Kiwi", "Orange"],
    };
  },
};
</script>

