<template>
  <div>
    <b-form>
      <div class="task-detail-form">
        <div class="font-input-box">
          <div class="input-heading">
            <h4>Task Details</h4>
            <div class="input-box mt-3">
              <label for="input-with-list">Project Name</label>
              <b-form-input placeholder="Team Page " type="text"></b-form-input>
            </div>
          </div>
          <div class="input-heading">
            <h4>Projects</h4>
            <div class="input-box arrow-selectar mt-3">
              <label for="input-with-list">Select Project</label>
              <b-form-input
                placeholder="In Progress"
                list="input-list"
                id="input-with-list"
              ></b-form-input>
              <b-form-datalist
                id="input-list"
                :options="options"
              ></b-form-datalist>
            </div>
          </div>
          <div class="input-heading width-min">
            <h4>Deadline</h4>
            <div class="input-box arrow-selectar mt-3 width">
              <label for="input-with-list">Date</label>
              <b-form-input
                placeholder="22/08/21"
                class="date-input"
                type="date"
              ></b-form-input>
            </div>
          </div>
          <div class="input-heading width-min mr-0">
            <h4>Status</h4>
            <div class="input-box arrow-selectar mt-3 width">
              <label for="input-with-list">Status</label>
              <b-form-input
                placeholder="In Progress"
                list="input-list"
                id="input-with-list"
              ></b-form-input>
              <b-form-datalist
                id="input-list"
                :options="options"
              ></b-form-datalist>
            </div>
          </div>
        </div>
        <div class="input-box mt-3">
          <label for="input-with-list">Description / Notes</label>

          <b-form-textarea
            id="textarea-rows"
            placeholder="Team Page "
            rows="5"
          ></b-form-textarea>
        </div>
      </div>
    </b-form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      options: [
        "English Transcription",
        "English Transcription",
        "English Transcription",
        "English Transcription",
        "English Transcription"
      ],
    };
  }
};
</script>

<style scoped>
.date-input {
  display: flex;
  flex-direction: row-reverse;
  padding: 0 !important;
}
.input-heading {
  width: 100%;
  margin-right: 10px;
}
.input-heading.width-min {
  max-width: 228px;
}
.task-detail-form label {
  position: absolute !important;
  top: -21px;
  left: -1px;
  background-color: #ffffff;
  font-size: 14px;
  color: #7d7d7d;
  font-weight: 500;
  z-index: 1;
}

.task-detail-form .form-group {
  position: relative;
  width: 48%;
}
.font-input-box {
  display: flex;
  justify-content: space-between;
  padding: 0 0 38px 0;
}

.input-heading h4 {
  font-size: 20px;
  color: #212121;
  font-weight: 400;
  margin: 0px 0 24px 0;
}
.task-detail-form .arrow-selectar:after {
  right: 0;
  top: 50%;
  width: 33px;
  height: 22px;
  transform: translate(-2px, -10%);
}
.task-detail-form .list-box {
  padding: 0;
}
.list-box .list-group {
  padding: 0px 0 28px 0;
}
.task-detail-form {
  padding: 20px 0px 0;
}
.task-detail-form input {
  height: 50px !important;
}
.task-detail-form .width input {
  width: 228px;
}
.task-detail-form .input-box {
  margin-top: 0 !important;
  display: inline-flex;
  position: relative;
  width: 100%;
}
textarea.form-control {
  padding: 13px 16px;
}
</style>
