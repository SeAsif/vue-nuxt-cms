<template>
  <div>
    <div class="service-setting">
      
      <h3 class="mt-4">Image</h3>
      <Upload />
      <div class="list-box">
        <h4>Position</h4>
        <b-list-group horizontal>
          <b-list-group-item
            ><b-link to="/"><b-img src="~assets/i/position-icon-1.svg" alt=""
          /></b-link></b-list-group-item>
          <b-list-group-item
            ><b-link to="/"><b-img src="~assets/i/position-icon-2.svg" alt=""
          /></b-link></b-list-group-item>
          <b-list-group-item
            ><b-link to="/"><b-img src="~assets/i/position-icon-3.svg" alt=""
          /></b-link></b-list-group-item>
          <b-list-group-item
            ><b-link to="/"><b-img src="~assets/i/position-icon-4.svg" alt=""
          /></b-link></b-list-group-item>
          <b-list-group-item
            ><b-link to="/"><b-img src="~assets/i/position-icon-5.svg" alt=""
          /></b-link></b-list-group-item>
          <b-list-group-item
            ><b-link to="/"><b-img src="~assets/i/position-icon-6.svg" alt=""
          /></b-link></b-list-group-item>
        </b-list-group>
      </div>
      <h5>Title</h5>
      <b-row>
        <b-col cols="12">
          <div class="input-box mt-2">
            <label for="input-with-list">Heading</label>
            <b-form-input
              placeholder="Transcription"
            type="text"
            ></b-form-input>
           
          </div>
        </b-col>
      </b-row>
      
      <div class="text-style">
        
         <div class="font-input-box">
          <h4>Font and Size</h4>
         <div class="input-box arrow-selectar mt-3">
            <b-form-input
              placeholder="Arial"
              list="input-list"
              id="input-with-list"
            ></b-form-input>
             <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
          </div>
             <div class="input-box arrow-selectar mt-3">
            <b-form-input
              placeholder="Regular"
              list="input-list"
              id="input-with-list"
            ></b-form-input>
             <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
          </div>
          <div class="input-box arrow-selectar mt-3 width">
            <b-form-input
              placeholder="14px"
              list="input-list"
              id="input-with-list"
            ></b-form-input>
            <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
          </div>
          </div>
            <div class="list-box">
            <h4>Position</h4>
            <b-list-group horizontal>
               <b-list-group-item
            ><b-link to="/"><b-img src="~assets/i/position-icon-1.svg" alt=""
          /></b-link></b-list-group-item>
          <b-list-group-item
            ><b-link to="/"><b-img src="~assets/i/position-icon-2.svg" alt=""
          /></b-link></b-list-group-item>
          <b-list-group-item class="pr-0"
            ><b-link to="/"><b-img src="~assets/i/position-icon-3.svg" alt=""
          /></b-link></b-list-group-item>
            </b-list-group></div>
        </div>
      <b-row>
        
        <b-col cols="12">
          <h5 class="mt-2">Description</h5>
          <div class="input-box mt-2">
            <label for="input-with-list">Message</label>
            <b-form-textarea
              placeholder="In today,s volatile and highly complex business environment, substantial"
              list="input-list"
              id="input-with-list"
            ></b-form-textarea>
          </div>
        </b-col>
      </b-row>
      <div class="text-style">
        
         <div class="font-input-box">
          <h4>Font and Size</h4>
         <div class="input-box arrow-selectar mt-3">
            <b-form-input
              placeholder="Arial"
              list="input-list"
              id="input-with-list"
            ></b-form-input>
             <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
          </div>
             <div class="input-box arrow-selectar mt-3">
            <b-form-input
              placeholder="Regular"
              list="input-list"
              id="input-with-list"
            ></b-form-input>
             <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
          </div>
          <div class="input-box arrow-selectar mt-3 width">
            <b-form-input
              placeholder="14px"
              list="input-list"
              id="input-with-list"
            ></b-form-input>
            <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
          </div>
          </div>
            <div class="list-box">
            <h4>Position</h4>
            <b-list-group horizontal>
               <b-list-group-item
            ><b-link to="/"><b-img src="~assets/i/position-icon-1.svg" alt=""
          /></b-link></b-list-group-item>
          <b-list-group-item
            ><b-link to="/"><b-img src="~assets/i/position-icon-2.svg" alt=""
          /></b-link></b-list-group-item>
          <b-list-group-item class="pr-0"
            ><b-link to="/"><b-img src="~assets/i/position-icon-3.svg" alt=""
          /></b-link></b-list-group-item>
            </b-list-group></div>
        </div>
            <div class="flex-btn">
        <b-button
          class="mt-3 create blue-btn"
          variant="primary"
          block
          >Add</b-button
        >
        <b-button
          class="mt-3 cancel"
          block
          >Cancel</b-button
        >
      </div>
    </div>
  </div>
</template>

<script>
import KeyWord from './Keyword.vue';
export default {
  components: { KeyWord },
  data() {
    return {
      options: [
        "Arial",
        "English Transcription",
        "English Transcription",
        "English Transcription",
        "English Transcription",
      ],
      value: ['Language', 'Published'],
      limit: 5
    };
  },
};
</script>

<style scoped>
.service-setting h3 {
  font-size: 20px;
  color: #212121;
  font-weight: 400;
  line-height: 23px;
}
.service-setting {
  background: #ffffff;
  box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.15), 0px 2px 5px rgba(0, 0, 0, 0.2);
  border-radius: 8px;
  padding: 23px 30px 30px;
}
.list-box .list-group-item {
  border: 0;
  padding: 0 12px 0 0px;
}
h4 {
  font-size: 14px;
  color: #212121;
  font-weight: 400;
  margin: 0 0 15px 0;
}
.service-setting h5 {
  font-size: 18px;
  color: #212121;
  font-weight: 400;
  margin: 0;
}

.list-box {
  padding: 22px 0 0 0;
}

.text-style .arrow-selectar:after {
    right: 3px;
    top: 14px;
    width: 23px;
    height: 10px;}
   .text-style .list-box {
        padding: 0;
}
.list-box .list-group {
    padding: 0px 0 28px 0;
}
.text-style {
    padding: 20px 0 0 0;
    display: flex;
    justify-content: space-between;
}
.text-style input {
    height: 32px !important;
        padding: 0 7px !important;
            width: 165px;}
       .text-style .width input{width: 80px;}
      .text-style .input-box {
    margin: 0 0 0 0;
        margin-top: 0 !important;
        display: inline-flex;
}
</style>