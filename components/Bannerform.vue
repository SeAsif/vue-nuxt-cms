<template>
  <div>
    <div class="tab-1">
      <div class="information-box information-box-scroll">
        <h4>General Information</h4>
        <div class="d-block text-center">
          <b-form>
            <b-row>
              <b-col cols="6">
                <div class="input-box">
                  <label for="input-with-list">Page Name</label>
                  <b-form-input
                    placeholder="Banner"
                    list="input-list"
                  ></b-form-input>
                </div>
              </b-col>
            </b-row>
            <div class="widgets text-left">
              <span>Widgets</span>
              <b-dropdown
                id="dropdown-offset"
                offset="25"
                text="..."
                class="m-2 dropdown-box"
              >
                <b-dropdown-item href="#">Action</b-dropdown-item>
                <b-dropdown-item href="#">Another action</b-dropdown-item>
                <b-dropdown-item href="#">Something else here</b-dropdown-item>
              </b-dropdown>
            </div>
            <div class="main-message">
              <div class="heading">
                <h3>Main Message</h3>
                <div class="icon-setting">
                  <b-button
                    to="/"
                    variant="outline-primary"
                    class="download-btn"
                  >
                    <b-img src="~assets/i/download.svg" />
                  </b-button>
                  <b-button
                    to="/"
                    variant="outline-primary"
                    class="download-btn"
                  >
                    <b-img src="~assets/i/settings-border.svg" />
                  </b-button>
                </div>
              </div>

              <div class="padding-box">
                <b-row>
                  <b-col cols="12">
                    <div class="input-box">
                      <label for="input-with-list">Heading</label>
                      <b-form-input
                        placeholder="Simplify the way you do business"
                        list="input-list"
                      ></b-form-input>
                    </div>
                  </b-col>
                </b-row>
                <b-row>
                  <b-col cols="12">
                    <div class="input-box">
                      <label for="input-with-list">Message</label>
                      <b-form-textarea
                        placeholder="GET STARTED"
                        list="input-list"
                      ></b-form-textarea>
                    </div>
                  </b-col>
                </b-row>

                <b-row>
                  <b-col cols="12">
                    <div class="input-box">
                      <label for="input-with-list">Button Text</label>
                      <b-form-input
                        placeholder="GET STARTED"
                        list="input-list"
                      ></b-form-input>
                    </div>
                  </b-col>
                </b-row>
              </div>
            </div>

            <div class="main-message">
              <div class="heading">
                <h3>Main Image</h3>
                <div class="icon-setting">
                  <b-button
                    to="/"
                    variant="outline-primary"
                    class="download-btn"
                  >
                    <b-img src="~assets/i/download.svg" />
                  </b-button>
                  <b-button
                    to="/"
                    variant="outline-primary"
                    class="download-btn"
                  >
                    <b-img src="~assets/i/settings-border.svg" />
                  </b-button>
                </div>
              </div>

              <div class="padding-box">
                <b-img src="~assets/i/main-img.png" />
              </div>
            </div>
            <div class="main-message">
              <div class="heading">
                <h3>Main Image</h3>
                <div class="icon-setting">
                  <b-button
                    to="/"
                    variant="outline-primary"
                    class="download-btn"
                  >
                    <b-img src="~assets/i/download.svg" />
                  </b-button>
                  <b-button
                    to="/"
                    variant="outline-primary"
                    class="download-btn"
                  >
                    <b-img src="~assets/i/settings-border.svg" />
                  </b-button>
                </div>
              </div>

              <div class="padding-box">
                <b-img src="~assets/i/shadow-img.png" />
              </div>
            </div>
          </b-form>
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
.input-box input,
.input-box textarea {
  border: 1px solid #e5e9ee;
  border-radius: 4px;
  height: 50px !important;
  padding: 0 18px !important;
}
.input-box textarea {
  height: 110px !important;
  padding: 13px 18px !important;
}
.input-box input::-webkit-input-placeholder {
  color: #212121;
}

.input-box input:-ms-input-placeholder {
  color: #212121;
}

.input-box input::placeholder {
  color: #212121;
}
.input-box textarea::-webkit-input-placeholder {
  color: #212121;
}

.input-box textarea:-ms-input-placeholder {
  color: #212121;
}

.input-box textarea::placeholder {
  color: #212121;
}
.information-box {
  border-radius: 4px;
  padding: 0 40px 24px 40px;
}
.information-box.information-box-scroll{
  padding: 22px 40px 24px 40px;

}
.widgets {
  display: flex;
  align-items: center;
  margin: 15px 0 15px;
}
.widgets span {
  font-weight: normal;
  font-size: 20px;
  color: #212121;
}
.download-btn {
  border: 0;
  padding: 0;
  margin: 0;
  margin-left: 6px;
}
.download-btn:hover {
  background-color: transparent !important;
}
.main-message .heading h3 {
  font-weight: normal;
  font-size: 18px;
  margin: 0;
}
</style>
