<template>
  <div>
    <b-modal id="bv-modal-example3" hide-footer>
      <template #modal-title>New Section </template>
      <div class="d-block text-center">
        <b-form>
          <div class="input-box arrow-selectar">
            <label for="input-with-list">Select Section</label>
            <b-form-input
              list="input-list"
              placeholder="Blog Slider"
              id="input-with-list"
            ></b-form-input>
            <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
          </div>
          <div class="input-box arrow-selectar">
            <label for="input-with-list">Heading</label>
            <b-form-input
              list="input-list"
              placeholder="Popular Posts"
              id="input-with-list"
            ></b-form-input>
            <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
          </div>

          <div class="quantity-box text-left">
            <label for="input-with-list">Posts Amount</label>
            <b-form-spinbutton
              id="sb-input"
              v-model="value1"
              @change="value2 = $event"
              wrap
            ></b-form-spinbutton>
          </div>

          <div class="input-box arrow-selectar nikepro-icon">
            <label for="input-with-list">Label</label>

            <b-form-input
              list="input-list"
              placeholder="Language/English/Transcription"
              id="input-with-list"
            ></b-form-input>
            <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
          </div>
          <div class="input-box arrow-selectar nikepro-icon">
            <label for="input-with-list">Label</label>

            <b-form-input
              list="input-list"
              placeholder="Language/Ukrainian/Transcription"
              id="input-with-list"
            ></b-form-input>
            <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
          </div>
        </b-form>
      </div>

      <div class="flex-btn">
        <b-button
          class="mt-3 create blue-btn"
          variant="primary"
          block
          @click="$bvModal.hide('bv-modal-example')"
          >Add</b-button
        >
        <b-button
          class="mt-3 cancel"
          block
          @click="$bvModal.hide('bv-modal-example')"
          >Cancel</b-button
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
</style>

<script>
export default {
  data() {
    return {
      options: ["Apple", "Banana", "Grape", "Kiwi", "Orange"],
      value1: 0,
      value2: null
    };
  }
};
</script>
