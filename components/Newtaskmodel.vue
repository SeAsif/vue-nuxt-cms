<template>
  <div>
    <b-modal size="lg" id="bv-modal-example" hide-footer>
      <template #modal-title>New Task</template>
      <div class="d-block text-center">
        <b-form>
          <b-row>
          <b-col lg="12">
            <b-row>
              <b-col lg="6" class="pr-4">
            <div class="input-box arrow-selectar">
              <label for="input-with-list">Task Name</label>
              <b-form-input
                list="input-list"
                placeholder="Add Team Page"
                id="input-with-list"
              ></b-form-input>
              <b-form-datalist
                id="input-list"
                :options="options"
              ></b-form-datalist>
            </div>
            <div class="input-box input-height">
              <label for="input-with-list">Heading</label>
              <b-form-textarea
    id="textarea-rows"
    placeholder="Data entry and market research"
    rows="8"
  ></b-form-textarea>
            </div>
            </b-col>
             <b-col lg="6" class="pl-4">
            <div class="input-box arrow-selectar">
              <label for="input-with-list">Select Project</label>
              <b-form-input
                list="input-list"
                placeholder="Team Page"
                id="input-with-list"
              ></b-form-input>
              <b-form-datalist
                id="input-list"
                :options="options"
              ></b-form-datalist>
            </div>
            <Upload/>
            </b-col>
            </b-row>
          </b-col>
          </b-row>
        </b-form>
      </div>
      <Newtaskblog />
      <b-col lg="6" class="pr-4 pl-0">
        <div class="flex-btn mt-3 mb-3">
          <b-button class="mt-3 create blue-btn" variant="primary" block
            >Add</b-button
          >
          <b-button class="mt-3 ml-3 cancel" block>Cancel</b-button>
        </div>
      </b-col>
    </b-modal>
  </div>
</template>
<style scoped>
.modal-header .modal-title {
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  color: #212121;
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
.flex-btn {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.flex-btn button.create {
  transition: all 0.6s;
}
.flex-btn button {
  height: 44px;
  width: 200px;
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
.modal-dialog {
  max-width: 477px I !important;
}
.modal-header {
  padding: 1rem 30px;
}
.modal-body {
  padding: 11px 30px 40px;
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
.nikepro-icon input {
  padding-left: 45px !important;
}
.input-box textarea.form-control {
        height: 270px;
    padding: 12px 17px 5px;
}
</style>

<script>
export default {
  data() {
    return {
      options: ["Task Page", "Task Page", "Task Page", "Task Page", "Task Page"]
    };
  }
};
</script>
