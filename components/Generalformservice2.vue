<template>
  <div>
    <div class="tab-1">
      <div class="back-btn"></div>
      <div class="information-box border-0">
        <div class="d-block text-center">
          <b-form>
            <b-row>
              <b-col cols="6">
                <b-col class="p-0">
                  <div class=" flex-dropdown text-left">
                    <h4>Service Settings</h4>
                    <b-dropdown
                      id="dropdown-offset"
                      offset="25"
                      text="..."
                      class=" dropdown-box"
                    >
                      <b-dropdown-item href="#">Action</b-dropdown-item>
                      <b-dropdown-item href="#">Another action</b-dropdown-item>
                      <b-dropdown-item href="#"
                        >Something else here</b-dropdown-item
                      >
                    </b-dropdown>
                  </div>
                  <div class="input-box">
                    <label for="input-with-list">Heading</label>
                    <b-form-input
                      placeholder="Services"
                      list="input-list"
                      id="input-with-list"
                    ></b-form-input>
                  </div>
                </b-col>

                <b-col class="p-0">
                  <div class="checkbox text-left">
                    <b-form-checkbox size="md">Use as Link</b-form-checkbox>
                  </div>
                  <div class="flex-btn">
                    <b-button
                      class="mt-3 create btn-blue"
                      variant="primary"
                      block
                      >Save Changes</b-button
                    >
                    <b-button class="mt-3 cancel ml-3" block>Cancel</b-button>
                  </div>
                </b-col>
              </b-col>
              <b-col cols="6">
                <b-col class="p-0">
                  <div class="text-flex flex-end text-left">
                    <b-form-checkbox-group
                      :options="options"
                      :aria-describedby="ariaDescribedby"
                      switches
                    ></b-form-checkbox-group>
                  </div>
                  <div class="input-box arrow-selectar arror-color">
                    <label for="input-with-list" style="opacity:0;"
                      >Select Viget</label
                    >
                    <b-form-input
                      disabled
                      placeholder="Select Page"
                      id="input-with-list"
                    ></b-form-input>
                  </div>
                </b-col>
              </b-col>
            </b-row>
          </b-form>

          <div class="sections-box sections-box2 text-left">
            <h4>Sections</h4>
            <b-button variant="primary" class="btn-blue"
              >Add New Section</b-button
            >
          </div>
          <Generalservicetable />
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
.flex-dropdown {
  display: flex;
  align-items: center;
}
.flex-dropdown h4 {
  margin-right: 15px;
}
.sections-box h4 {
  margin: 47px 0 57px;
}
.sections-box.sections-box2 {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin: 47px 0 40px;
}
.sections-box.sections-box2 h4 {
  margin: 0;
}
</style>

<script>
export default {
  data() {
    return {
      selected: [],
      options: [{ text: "", value: "red" }]
    };
  }
};
</script>
