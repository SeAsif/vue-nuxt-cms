<template>
  <div>
    <b-modal id="bv-modal-example" hide-footer>
      <template #modal-title>New Site</template>
      <div class="d-block text-center">
        <b-form>
          <div class="input-box">
            <label for="input-with-list">Site Name</label>
            <b-form-input
              placeholder="Nike Pro"
              list="input-list"
            ></b-form-input>
          </div>
          <div class="input-box">
            <label for="input-with-list">URL</label>
            <b-form-input
              placeholder="www.nilepro.com"
              list="input-list"
            ></b-form-input>
          </div>
        </b-form>
      </div>
      <div class="upload-file">
        <b-img src="~assets/i/drag.svg" />
        <h4>Drag and drop your site logo here</h4>
        <div class="upload-btn">
          <p>Upload</p>
          <b-form-file v-model="file2" class="mt-3" plain></b-form-file>
        </div>
      </div>

      <div class="flex-btn mb-3">
                <b-button
          class="mt-3 cancel"
          block
          @click="$bvModal.hide('bv-modal-example')"
          >Cancel</b-button
        >
        <b-button
          class="mt-3 create btn-blue"
          variant="primary"
          block
          @click="$bvModal.hide('bv-modal-example')"
          >Create</b-button
        >

      </div>
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
.modal-dialog {
  max-width: 477px I !important;
}
.modal-header {
  padding: 1rem 30px;
}
.modal-body {
  padding: 11px 30px 40px;
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
  cursor: pointer;
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
</style>

<script>
export default {
  data() {
    return {
      options: ["Apple", "Banana", "Grape", "Kiwi", "Orange"]
    };
  }
};
</script>
