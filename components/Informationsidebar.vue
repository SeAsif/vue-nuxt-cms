<template>
  <div>
    <div class="information-sidebar">
      <div class="chat-box">
        <h1 class="m-0">Information</h1>
      </div>
      <div class="vlad-box text-center">
        <div class="img-box">
          <img src="~assets/i/vlad.svg" />
        </div>
        <h4>Vlad Sklyar</h4>
      </div>
      <div class="content-box">
        <h4>Content:</h4>
        <div class="photos-box">
          <span
            ><img src="~assets/i/photos.svg" />
            <p>Photos:</p></span
          >
          <strong>22</strong>
        </div>
        <div class="photos-box">
          <span
            ><img src="~assets/i/files.svg" />
            <p>Files:</p></span
          >
          <strong>344</strong>
        </div>
        <div class="photos-box">
          <span
            ><img src="~assets/i/links.svg" />
            <p>Links:</p></span
          >
          <strong>99</strong>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.chat-box {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px 20px 16px 15px;
}
.chat-box h1 {
  font-weight: normal;
  font-size: 24px;
  color: #212121;
}
.information-sidebar .chat-box {
  border-bottom: 1px solid #e5e9ee;
}
.vlad-box h4 {
  font-style: normal;
  font-weight: 500;
  font-size: 15px;
  margin-top: 12px;
}
.vlad-box .img-box {
  width: 100px;
  height: 100px;
  border-radius: 100%;
  overflow: hidden;
  margin: 0 auto;
}
.vlad-box {
  padding: 47px 0;
  border-bottom: 1px solid #e5e9ee;
}
.content-box .photos-box {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 16px;
}
.content-box .photos-box span {
  display: flex;
  align-items: center;
}
.content-box .photos-box span p {
  margin: 0;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  color: #212121;
  margin-left: 13px;
}
.content-box .photos-box strong {
  font-weight: 500;
  font-size: 14px;
  color: #4489fe;
  text-decoration: underline;
}
.content-box h4 {
  font-style: normal;
  font-weight: 500;
  font-size: 15px;
  margin-top: 12px;
  margin: 22px 0 17px;
}
.content-box {
  padding-left: 15px;
}
</style>
