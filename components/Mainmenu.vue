<template>
  <div>
    <div class="general-settings-page">
      <h3>Main Menu</h3>
      <b-button block variant="primary" class="text-left general-btn"
        ><b-img src="~assets/i/statistics.svg" />Statistics</b-button
      >

      
      
       <div class="levels">
        <b-button
          :class="visible ? null : 'collapsed'"
          :aria-expanded="visible ? 'true' : 'false'"
          aria-controls="collapse"
          class="arrow-selectar"
          @click="visible = !visible"
        >
        
    <b-img src="~assets/i/team.svg" />
         <span> Team</span>
        </b-button>
        <b-collapse id="collapse" v-model="visible">
          <b-list-group-item >
              
               <b-list-group>
        <b-list-group-item button>Staff</b-list-group-item>
        <b-list-group-item button>Tasks</b-list-group-item>
        <b-list-group-item button>Archieve</b-list-group-item>
        
      </b-list-group> 
              </b-list-group-item>
        </b-collapse>
      </div>
      <div class="levels">
        <b-button
          :class="visibleone ? null : 'collapsed'"
          :aria-expanded="visibleone ? 'true' : 'false'"
          aria-controls="collapse-1"
          class="arrow-selectar"
          @click="visibleone = !visibleone"
        >
        
    <b-img src="~assets/i/client.svg" />
         <span> Clients</span>
        </b-button>
        <b-collapse id="collapse-1" v-model="visibleone">
          <b-list-group-item >
              
               <b-list-group>
          <b-list-group-item button>Staff</b-list-group-item>
        <b-list-group-item button>Tasks</b-list-group-item>
        <b-list-group-item button>Archieve</b-list-group-item>
        
      </b-list-group> 
              </b-list-group-item>
        </b-collapse>
      </div>
    <div class="levels">
        <b-button
          :class="visibletwo ? null : 'collapsed'"
          :aria-expanded="visibletwo ? 'true' : 'false'"
          aria-controls="collapse-2"
          class="arrow-selectar"
          @click="visibletwo = !visibletwo"
        >
        
    <b-img src="~assets/i/integration.svg" />
         <span> Integration</span>
        </b-button>
        <b-collapse id="collapse-2" v-model="visibletwo">
          <b-list-group-item >
              
               <b-list-group>
         <b-list-group-item button>Staff</b-list-group-item>
        <b-list-group-item button>Tasks</b-list-group-item>
        <b-list-group-item button>Archieve</b-list-group-item>
        
      </b-list-group> 
              </b-list-group-item>
        </b-collapse>
      </div>
      <div class="levels">
        <b-button
          :class="visiblethree ? null : 'collapsed'"
          :aria-expanded="visiblethree ? 'true' : 'false'"
          aria-controls="collapse-3"
          class="arrow-selectar"
          @click="visiblethree = !visiblethree"
        >
        
    <b-img src="~assets/i/payment.svg" />
         <span> Payments</span>
        </b-button>
        <b-collapse id="collapse-3" v-model="visiblethree">
          <b-list-group-item >
              
               <b-list-group>
        <b-list-group-item button>Staff</b-list-group-item>
        <b-list-group-item button>Tasks</b-list-group-item>
        <b-list-group-item button>Archieve</b-list-group-item>
        
      </b-list-group> 
              </b-list-group-item>
        </b-collapse>
      </div>
      <div class="levels">
        <b-button
          :class="visiblefour ? null : 'collapsed'"
          :aria-expanded="visiblefour ? 'true' : 'false'"
          aria-controls="collapse-4"
          class="arrow-selectar"
          @click="visiblefour = !visiblefour"
        >
        
    <b-img src="~assets/i/setting-black-icon.svg" />
         <span> Settings</span>
        </b-button>
        <b-collapse id="collapse-4" v-model="visiblefour">
          <b-list-group-item >
              
               <b-list-group>
         <b-list-group-item button>Staff</b-list-group-item>
        <b-list-group-item button>Tasks</b-list-group-item>
        <b-list-group-item button>Archieve</b-list-group-item>
        
      </b-list-group> 
              </b-list-group-item>
        </b-collapse>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      visible: true,
      visibleone: false,
      visibletwo: false,
      visiblethree: false,
      visiblefour: false,

    };
  },
};
</script>
<style scoped>
.levels button {
    width: 100%;
    text-align: left;
    background-color: transparent !important;
    font-size: 14px;
    color: #212121;
    border: 0;
    padding: 12px 12px;
}
.levels button:active{box-shadow: none !important;}
.levels button:focus{box-shadow: none !important;}
.levels .list-group-item {
    border: 0;
    padding: 4px 0 20px;
}
.general-settings-page {
      border-right: 1px solid #e5e9ee;
  padding: 22px 15px;
}
.general-settings-page h3 {
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 0px 7px 16px;
}
.general-settings-page .btn-primary.general-btn {
  background: #e9f0fd;
  border-radius: 8px;
  border: 0;
  color: #4489fe;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  padding: 15px 16px;
  display: flex;
  align-items: center;
}
.general-settings-page .btn-blue {
  width: 220px;
  height: 44px;
  margin: 19px auto 0;
}
.general-settings-page img {
  margin-right: 17px;
}
.general-settings-page h3 img {
  margin-right: 14px;
}
.general-settings-page .menu-btn {
  background: none;
  border: 0;
  color: #212121;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
}
.general-settings-page .list-group button {
border: 0;
    color: #212121;
    font-weight: normal;
    font-size: 14px;
    border-radius: 8px;
    padding: 14px 11px;
}
.general-settings-page .list-group button:after {
  position: absolute;
  content: "";
  left: -14px;
  top: 24px;
  width: 20px;
  height: 1px;
  background-repeat: no-repeat;
  pointer-events: none;
  background: #e5e9ee;
}
.general-settings-page .list-group {
  border-left: 1px solid #e5e9ee;
    margin-left: 21px;
    padding-left: 14px;
}
.general-settings-page.arrow-selectar:after {
  top: 15px;
  background-color: transparent !important;
}
.levels .arrow-selectar:after {
    top: 21px;
}
.general-settings-page .list-group button:last-child {
    padding-bottom: 0px;
    line-height: 2px;
    padding-top: 25px;
}
.levels span {
    color: #212121;
    font-size: 14px;
    font-weight: 500;
}
</style>
