<template>
  <div>
    <b-container>
      <b-row>
        <b-col col="3" lg="3" class="pl-0 search-bar-two">
          <Searchbar />
        </b-col>

        <b-col col="9" lg="9">
          <div class="transcription-services d-flex">
            <b-list-group>
              <b-list-group-item>
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/"
                  >Legal Transcription Services</b-link
                ><b-img src="~assets/i/cross.svg" alt="" />
              </b-list-group-item>
              <b-list-group-item>
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" to="/">Home Page-</b-link
                ><b-img src="~assets/i/cross.svg" alt="" />
              </b-list-group-item>
              <b-list-group-item>
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/"
                  >Interview Transcription
                </b-link>
                <b-img src="~assets/i/cross.svg" alt="" />
              </b-list-group-item>
               <b-list-group-item>
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/"
                  >Academic Transcription Service
                </b-link>
                <b-img src="~assets/i/cross.svg" alt="" />
              </b-list-group-item>
            </b-list-group>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap");
.nikepro-box .list-group {
  display: flex;
  width: 100%;
  flex-direction: row;
}

.nikepro-box .list-group .list-group-item {
  border: none;
  padding: 0;
  margin: 0;
}

.list-group-item img {
  margin: 0 4px;
}
.nikepro-box img {
  margin: 0 20px 0 5px;
  height: 13px;
  width: 15px;
}
.nikepro-box img:lastchild {
  margin: 0px;
}
.list-group-item a {
  color: #212121;
  font-family: Roboto;
  font-style: normal;
  font-weight: 500;
  font-size: 13px;
  text-decoration: none;
  line-height: 16px;
}
.nikepro-box {
  border-bottom: 1px solid #e5e9ee;
  padding: 15px 0;
}
.transcription-services .list-group {
  flex-direction: row;
}

.transcription-services .list-group-item {
  padding: 7px 0;
  margin: 0 7px;
  border: 0;
}
.transcription-services {
  padding: 8px 0;
  border-bottom: 1px solid #e5e9ee;
}
.transcription-services .list-group-item a {
  font-weight: 400;
}
.transcription-services .list-group-item img {
  margin: 0 10px;
}
.transcription-services .list-group-item:hover {
  background-color: #e9f0fd;
  border-radius: 8px;
}
.transcription-services .list-group-item::after {
  content: "";
  border-right: 1px solid #e5e9ee !important;
  position: absolute;
  right: -7px;
  top: 0;
  bottom: 0;
}
.nike-img img {
  margin-right: 12px;
}
.nikepro-box .list-group .list-group-item img {
  margin: 0 12px 0 10px;
  width: 12px;
  height: 12px;
}
</style>
