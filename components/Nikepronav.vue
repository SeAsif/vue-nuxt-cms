<template>
  <div>
    <div class="nikepronav">
    <b-container>
      <b-row>
        <b-col sm="5" class="pr-0">
          <div class="nikepro-box d-flex align-items-center">
            <b-link rel="stylesheet" to="/"><b-img src="~assets/i/arrow-back.svg" alt="" /></b-link>
            <b-link rel="stylesheet" to="/"><b-img src="~assets/i/arrow-next.svg" alt="" /></b-link>
            <b-link rel="stylesheet" to="/"><b-img src="~assets/i/arrow-up.svg" alt="" /></b-link>
           <b-link class="nike-img" rel="stylesheet" to="/"><b-img src="~assets/i/nikepro-img.svg" alt="" /></b-link>
            <b-list-group>



              <b-list-group-item>
                <b-link rel="stylesheet" to="/">  NikePro</b-link>
                <b-img src="~assets/i/blue-next-arrow.svg" alt="" />
              </b-list-group-item>
              <b-list-group-item>
                <b-link rel="stylesheet" to="/"> Languages</b-link>
                <b-img src="~assets/i/blue-next-arrow.svg" alt="" />
              </b-list-group-item>
              <b-list-group-item><b-link rel="stylesheet" to="/"> Ukraine</b-link>
              </b-list-group-item>
            </b-list-group>
          </div>
        </b-col>

        <b-col sm="7">
          <div class="transcription-services d-flex">
            <b-list-group class="tabsflexible">
              <b-list-group-item>
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" to="/">Legal Transcription Services</b-link><b-img src="~assets/i/cross.svg" alt="" />
              </b-list-group-item>
              <b-list-group-item>
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" to="/">Home Page-</b-link><b-img src="~assets/i/cross.svg" alt="" />
              </b-list-group-item>
              <b-list-group-item>
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" to="/">Interview Transcription </b-link>
                <b-img src="~assets/i/cross.svg" alt="" />
              </b-list-group-item>
               <b-list-group-item>
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" to="/">Home Page-</b-link><b-img src="~assets/i/cross.svg" alt="" />
              </b-list-group-item>
                        
            </b-list-group>
          </div>
        </b-col>
      </b-row>
      </b-container>
    </div>
    </div>
  
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap');

.tabsflexible{
  display: -webkit-box;
    padding-left: 0;
    margin-bottom: 0;
    border-radius: 0.25rem;
    width: 100%;
    flex-direction: unset !important;
    flex-wrap: unset;
    
}
.tabsflexible .list-group-item{
  padding: 7px 0;
    margin: 0 7px;
    border: 0;
    -webkit-box-flex: 1;
    white-space: nowrap;
    overflow: hidden;
    border-bottom: none;
    text-overflow: ellipsis;
    padding-right: 20px !important;
}
.tabsflexible .list-group-item img:last-child{
      position: absolute;
    right: -4px;
    top: 14px;
    cursor: pointer;
}
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
        margin: 0 13px 0 5px;
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
    font-size: 14px;
    text-decoration: none;
    line-height: 16px;
}
.nikepro-box {
        border-bottom: 1px solid #e5e9ee;
    padding: 15px 0;
    height: 100%;
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
    font-weight: 400;}
    .transcription-services .list-group-item img {
    margin: 0 10px;
}
.transcription-services .list-group-item:hover {
    background-color: #E9F0FD;
    border-radius: 8px;
}
.transcription-services .list-group-item::after{      content: "";
    border-right: 1px solid #e5e9ee !important;
    position: absolute;
    right: -7px;
    top: 0;
    bottom: 0;}
    .nike-img img{margin-right: 12px;}
    .nikepro-box .list-group .list-group-item img {
    margin: 0 7px 0 3px;
    width: 12px;
    height: 12px;
}
</style>