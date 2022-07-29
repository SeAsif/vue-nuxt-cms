<template>
  <div>
    <b-container fluid>
      <div class="general-setting">
        <h3>General Settings</h3>
        <b-form>
          <div class="position-relative mb--4">
            <label for="input-with-list">Page Name</label>
            <b-form-input type="text" placeholder="Page Name" id=""></b-form-input>
          </div>
          <div class="position-relative">
            <label for="input-with-list">URL</label>
            <b-form-input
              type="text"
              placeholder="URL"
              id=""
            ></b-form-input>
          </div>
          <div class="position-relative mb--4">
            <label for="input-with-list">META Title</label>
            <b-form-input type="text" placeholder="Select Title" id=""></b-form-input>
          </div>
          <div class="position-relative text-area w-100 mb--4 ">
            <label for="input-with-list">META Description</label>
            <b-form-textarea
    id="textarea-no-resize"
    placeholder="Enter Meta Decription"
    rows="5"
    no-resize
  ></b-form-textarea>
           
          </div>
           <div class="position-relative w-100 mb-3 add-tags">
            
          <label for="tags-limit">Keywords</label>

          <Keyword />
          </div>
             
                 <div class="header-footer-input">
                     <h3>Header Settings</h3>
                <div class="position-relative input-height box-white ">
            <label for="input-with-list">Header</label>
            <b-img src="~assets/i/nikepro-img.svg" alt="" />
              <b-form-input no-caret 
              append-icon=""
              list="input-list"
              placeholder="Select Header"
              id="input-with-list"
            ></b-form-input>

            <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
          </div>


          
          
         </div>
         <div class="header-footer-input">
                  <h3>Footer Settings</h3>
            <div class="position-relative input-height box-white">
            <label for="input-with-list">Footer</label>
            <b-img src="~assets/i/nikepro-img.svg" alt="" />
            <b-form-input
              list="input-list"
              placeholder="Select Footer"
              id="input-with-list"
            ></b-form-input>
            
            <b-form-datalist
              id="input-list"
              :options="options"
            ></b-form-datalist>
           
          </div>
         </div>
         <div class="form-btn">
         <b-button class="btn-one" >Save Changes</b-button>
         <b-button class="btn-two" >Cancel</b-button>
         </div>
        </b-form>
      </div>
    </b-container>
  </div>
</template>


<script>
export default {
  data() {
    return {
      options: ["Apple", "Banana", "Grape", "Kiwi", "Orange"],
    };
  },
};
</script>


<style scoped>
input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0;
}
input:hover::-webkit-outer-spin-button,
input:hover::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0;
}
.b-form-tag {
    font-size: 75%;
    font-weight: normal;
    line-height: 1.5;
    margin-right: 1.25rem;
}

body > .tagStyle{
    background-color: tomato;
}
.general-setting label {
  position: absolute !important;
  top: -10px;
  left: 19px;
  background-color: #ffffff;
  font-size: 14px;
  color: #7d7d7d;
  font-weight: 500;
  z-index: 1;
}

.general-setting .form-group {
  position: relative;
  width: 48%;
}
.general-setting .form-control {
  height: 50px;
  line-height: 50px;
  color: #212121;
  font-size: 14px;
  font-weight: 400;
}
.general-setting form {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
#input-with-list {
  background-image: url(assets/i/select-arrow.svg);
  height: 50px;
  line-height: 28px;
  background-repeat: no-repeat;
  background-position: 80% 50%;
  cursor: pointer;
  font-size: 14px;
    font-weight: 400;
}
#bg-img{background-image: url(assets/i/select-arrow.svg);
  height: 50px;
  line-height: 28px;
  background-repeat: no-repeat;
  background-position: 80% 50%;
  cursor: pointer;}
.general-setting .position-relative {
  width: 48.5%;
}
.general-setting .position-relative button {
position: absolute;
    top: 50%;
    transform: translate(-19px, -50%);
    right: 0;
    border: 0;
    background: #ffffff;}

/* .general-setting .position-relative img {
  position: absolute;
  top: 8px;
  right: 16px;
  border: 1px solid #e5e9ee;
  padding: 8px 8px;
  border-radius: 4px;
  background: #ffffff;
} */
.select-input {
  margin: 0 0 38px 0;
}
.mb--4 {
  margin: 0 0 40px 0;
}
.general-setting h3 {
  font-size: 20px;
  line-height: 35px;
  font-weight: 400;
  margin: 0 0 24px 0;
}
.general-setting {
  padding: 16px 13px 0;
  padding-right: 0;
}
.add-tags .b-form-tags-button {
    display: none !important;}
.badge-secondary {
    color: #4489FE;
    background-color: #E9F0FD;
    width: 98px;
    height: 27px;
}
.text-truncate {
    line-height: 23px;
}
.general-setting .position-relative.add-tags img {
    top: 50%;
    transform: translate(0, -50%);
}
.btn-outline-secondary:not(:disabled):not(.disabled):active, .btn-outline-secondary:not(:disabled):not(.disabled).active, .show > .btn-outline-secondary.dropdown-toggle {
    display: none !important;
}
.invisible {
    visibility: hidden;
}
.general-setting .add-tags .form-control {
    height: 122px !important;
}
.input-height input{height: 122px;}
#textarea-no-resize {
    height: 122px;
}
.general-setting .position-relative.text-area button {
    top: 50%;
    transform: translate(-14px, -50%);
    right: 0;
}
#textarea-no-resize {
    height: 122px;
    padding: 20px 98px 0 13px;
    line-height: 20px;
    /* background-image: url(assets/i/select-arrow.svg); */
    background-position: 90% 50%;
    cursor: pointer;
    background-repeat: no-repeat;
}
.header-footer-input {
    width: 48.5%;
}
.header-footer-input .position-relative {
    width: unset;
}
btn{padding: 13px 45px;}
.form-btn button.btn {
    width: 170px;
    height: 44px;
    margin: 0 9px 40px 0px;
    font-size: 14px;
    font-weight: 500;
}
.form-btn{ padding: 30px 0 0 0;}
button.btn.btn-one {
    background-color: #4489FE;
    color: #ffffff;
    border: none;
}
button.btn.btn-two{
    color: #7D7D7D;
    background-color: #ffffff;
    border: 1px solid #DEE0E4;
}
.header-footer-input input{background-image: url(assets/i/select-arrow.svg);
    height: 50px;
    line-height: 28px;
    background-repeat: no-repeat;
    background-position: 95% 50%;
    cursor: pointer;}
    .header-footer-input #input-with-list {
    background-position: 95% 50%;
    padding: 0 49px;
}



.general-setting input::-webkit-input-placeholder {
  color: #212121;
}

.general-setting input:-ms-input-placeholder {
  color: #212121;
}

.general-setting input::placeholder {
  color: #212121;
}
.header-footer-input .position-relative img {
    position: absolute;
    top: 50%;
    left: 0;
    transform: translate(20px, -50%);
}
</style>