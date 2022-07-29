<template>
  <div>
    <div class="scroll-sidebar">
    <h2>Directory</h2>
    <div class="levels levelone">
    <b-button
    
      :class="visible ? null : 'collapsed'"
      :aria-expanded="visible ? 'true' : 'false'"
      aria-controls="collapse-1"
      @click="visible = !visible"
      
    >
    <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img class="home-pic" src="~assets/i/home-img.svg" alt="" />
      <span>Site</span>  
    </b-button>
    </div>
    <b-collapse id="collapse-1" v-model="visible" class="mt-2">

      <div class="levels leveltwo">
        <b-button
          :class="visibletwo ? null : 'collapsed'"
          :aria-expanded="visibletwo ? 'true' : 'false'"
          aria-controls="collapse-2"
          @click="visibletwo = !visibletwo"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
         <span> Transcription</span>
        </b-button>
        <b-collapse id="collapse-2" v-model="visibletwo" class="mt-2">

            <div class="levels levelthree">
        <b-button
          :class="visibleeight ? null : 'collapsed'"
          :aria-expanded="visibleeight ? 'true' : 'false'"
          aria-controls="collapse-8"
          @click="visibleeight = !visibleeight"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
         <span> English</span>
        </b-button>
        <b-collapse id="collapse-8" v-model="visibleeight" class="mt-2">
           <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/">Legal Transcription Services</b-link> 
              </b-list-group-item>
        </b-collapse>
      </div>
        <div class="levels levelthree">
        <b-button
          :class="visiblenine ? null : 'collapsed'"
          :aria-expanded="visiblenine ? 'true' : 'false'"
          aria-controls="collapse-9"
          @click="visiblenine = !visiblenine"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
         <span> Russian</span>
        </b-button>
        <b-collapse id="collapse-9" v-model="visiblenine" class="mt-2">
           <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/">Legal Transcription Services</b-link> 
              </b-list-group-item>
        </b-collapse>
      </div>
        <div class="levels levelthree">
        <b-button
          :class="visibleten ? null : 'collapsed'"
          :aria-expanded="visibleten ? 'true' : 'false'"
          aria-controls="collapse-10"
          @click="visibleten = !visibleten"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
         <span> Ukrainian</span>
        </b-button>
        <b-collapse id="collapse-10" v-model="visibleten" class="mt-2">
           <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/">Legal Transcription Services</b-link> 
              </b-list-group-item>
        </b-collapse>
      </div>

        </b-collapse>
      </div>

      <div class="levels leveltwo">
        <b-button
          :class="visiblethree ? null : 'collapsed'"
          :aria-expanded="visiblethree ? 'true' : 'false'"
          aria-controls="collapse-3"
          @click="visiblethree = !visiblethree"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
         <span> Video</span>
        </b-button>
        <b-collapse id="collapse-3" v-model="visiblethree" class="mt-2">
          <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/">Legal Transcription Services</b-link> 
              </b-list-group-item>
        </b-collapse>
      </div>

      <div class="levels leveltwo">
        <b-button
          :class="visiblefour ? null : 'collapsed'"
          :aria-expanded="visiblefour ? 'true' : 'false'"
          aria-controls="collapse-4"
          @click="visiblefour = !visiblefour"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
         <span> Images</span>
        </b-button>
        <b-collapse id="collapse-4" v-model="visiblefour" class="mt-2">
          <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/">Legal Transcription Services</b-link> 
              </b-list-group-item>
        </b-collapse>
      </div>

      <div class="levels leveltwo">
        <b-button
          :class="visiblefive ? null : 'collapsed'"
          :aria-expanded="visiblefive ? 'true' : 'false'"
          aria-controls="collapse-5"
          @click="visiblefive = !visiblefive"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
          <span>Text</span>
        </b-button>
        <b-collapse id="collapse-5" v-model="visiblefive" class="mt-2">
           <div class="levels levelthree">
        <b-button
          :class="visibleeleven ? null : 'collapsed'"
          :aria-expanded="visibleeleven ? 'true' : 'false'"
          aria-controls="collapse-11"
          @click="visibleeleven = !visibleeleven"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
          <span>Folder</span>
        </b-button>
        <b-collapse id="collapse-11" v-model="visibleeleven" class="mt-2">
          <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/">Legal Transcription Services</b-link> 
              </b-list-group-item>
              <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" /><a href="#"
                  >Academic Transcription </a> 
              </b-list-group-item>
              <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" /><a href="#"
                  >Interview Transcription</a> 
              </b-list-group-item>
        </b-collapse>
      </div>
        </b-collapse>
      </div>

      <div class="levels leveltwo">
        <b-button
          :class="visiblesix ? null : 'collapsed'"
          :aria-expanded="visiblesix ? 'true' : 'false'"
          aria-controls="collapse-6"
          @click="visiblesix = !visiblesix"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
          <span>Files</span>
        </b-button>
        <b-collapse id="collapse-6" v-model="visiblesix" class="mt-2">
           <div class="levels levelthree">
        <b-button
          :class="visibletewelve ? null : 'collapsed'"
          :aria-expanded="visibletewelve ? 'true' : 'false'"
          aria-controls="collapse-12"
          @click="visibletewelve = !visibletewelve"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
          <span>SVG</span>
        </b-button>
        <b-collapse id="collapse-12" v-model="visibletewelve" class="mt-2">
         <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/">Legal Transcription Services</b-link> 
              </b-list-group-item>
        </b-collapse>
      </div>
        <div class="levels levelthree">
        <b-button
          :class="visiblethirteen ? null : 'collapsed'"
          :aria-expanded="visiblethirteen ? 'true' : 'false'"
          aria-controls="collapse-13"
          @click="visiblethirteen = !visiblethirteen"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
          <span>PDF</span>
        </b-button>
        <b-collapse id="collapse-13" v-model="visiblethirteen" class="mt-2">
         <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/">Legal Transcription Services</b-link> 
              </b-list-group-item>
        </b-collapse>
      </div>
        <div class="levels levelthree">
        <b-button
          :class="visiblefourteen ? null : 'collapsed'"
          :aria-expanded="visiblefourteen ? 'true' : 'false'"
          aria-controls="collapse-14"
          @click="visiblefourteen = !visiblefourteen"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
          <span>PNG</span>
        </b-button>
        <b-collapse id="collapse-14" v-model="visiblefourteen" class="mt-2">
         <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/">Legal Transcription Services</b-link> 
              </b-list-group-item>
        </b-collapse>
      </div>
        </b-collapse>
      </div>
      
      <div class="levels leveltwo">
        <b-button
          :class="visibleseven ? null : 'collapsed'"
          :aria-expanded="visibleseven ? 'true' : 'false'"
          aria-controls="collapse-7"
          @click="visibleseven = !visibleseven"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
          <span>Links</span>
        </b-button>
        <b-collapse id="collapse-7" v-model="visibleseven" class="mt-2">
            <div class="levels levelthree">
        <b-button
          :class="visiblefifteen ? null : 'collapsed'"
          :aria-expanded="visiblefifteen ? 'true' : 'false'"
          aria-controls="collapse-15"
          @click="visiblefifteen = !visiblefifteen"
        >
        <b-img src="~assets/i/arrow-down-blue.svg" alt="" />
    <b-img src="~assets/i/nikepro-img.svg" alt="" />
          <span>Pages Links</span>
        </b-button>
        <b-collapse id="collapse-15" v-model="visiblefifteen" class="mt-2">
         <b-list-group-item >
                <b-img src="~assets/i/paper.svg" alt="" />
                <b-link rel="stylesheet" href="/">Legal Transcription Services</b-link> 
              </b-list-group-item>
        </b-collapse>
      </div>
        </b-collapse>
      </div>
    </b-collapse>
  </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      visible: true,
      visibletwo: true,
      visiblethree: false,
      visiblefour: false,
      visiblefive: true,
      visiblesix: true,
      visibleseven: true,
       visibleeight: false,
      visiblenine: false,
      visibleten: false,
      visibleeleven: true,
      visibletewelve: false,
       visiblethirteen: false,
        visiblefourteen: false,
        visiblefifteen: true,
    };
  },
};
</script>
<style scoped>
body{font-family: 'Roboto';}
h2{font-size: 18px;
line-height: 21px;
font-weight: 400;
color: #212121;
padding: 16px 18px 5px;
    margin: 0;
}
img.home-pic {
    height: 23px;
}
.levels button {
    color: #212121;
    background-color: #ffffff;
    border: none;
    font-size: 14px;
    line-height: 16px;
    font-weight: 400;
    display: flex;
    align-items: center;
}
.levels button:hover {
  background-color: unset;
  border: unset;
  color: unset;
}
.levels button:active {
  background-color: transparent !important;
  border: transparent;
  color: unset !important;
  outline: none !important;
}
.levels button:focus{ outline: none !important; box-shadow: none;}
.leveltwo img{padding:0 0 0 10px}
.levels span {
    margin: 0 0 0 7px;
}
.levels.levelthree {
    padding: 5px 0 5px 17px;
}
.levels .list-group-item {
    padding: 0;
    font-size: 13px;
    border: none;
    font-weight: 400;
}
.levels .list-group-item a {
    color: #212121;
    padding: 0 9px;
    text-decoration: none;
}
.levels .list-group-item img {
    padding: 0;
}
.levelthree .list-group-item {
    margin: 0 0 0 25px !important;
    padding: 13px 0 13px 14px;
}
.levels.leveltwo {
    padding: 5px 7px;
}
.levelthree .list-group-item:hover{ background-color: #E9F0FD; border-radius: 8px;}
.levelone button img {
    padding: 0 0 0 5px;
}
.levels button {
      padding: 6px 33px;
      position: relative;
}
.leveltwo .list-group-item[data-v-918615bc] {
    margin: 0 0 0 30px !important;
    padding: 13px 0 13px 14px;
    width: 100%;
    display: flex;
    align-items: center;
}
</style>