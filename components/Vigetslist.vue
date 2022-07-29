<template>
  <div>
    <div class="tab-2 d-none" :class="{ active: isActive2 }">
      <div class="back-btn"></div>
      <div class="information-box widgetMainScroll activity-main" id="scrolltopm">
        <div class="activity-box bg-white pt-2">
          <div class="vigets-list">
            <h4>Widgets List</h4>
            <b-button v-on:click="craetePage()" variant="primary" class="btn-blue"
              >Add New Widget</b-button
            >
          </div>
          <div class="form-box">
            <b-nav-form>
              <b-form-input
                size="sm"
                class="mr-sm-2"
                placeholder="Search"
              ></b-form-input>
            </b-nav-form>
            <div class="sort-box">
              <button>
                <span>Sort</span> <b-img src="~assets/i/vector.svg" />
              </button>
              <button>
                <span>Filter</span> <b-img src="~assets/i/vector.svg" />
              </button>
            </div>
          </div>
        </div>
        <Vigetstable/>
        <!-- <Pagination/> -->
      </div>
    </div>

     <div class="d-none" :class="{ active: isActive }"><CreateWidgets /></div>

  </div>
</template>
<script>
  export default {
    data() {
    return{
      isActive: false,
      isActive2: true
      }
    },
    methods: {
    craetePage: function () {
      this.isActive = !this.isActive;
      this.isActive2 = !this.isActive2;
    }
  }
  }
</script>
<style>
.activity-box{
  /* position: sticky;
  top: 0;
  z-index: 1;
  padding-top: 20px;
  padding-bottom: 10px; */
}
.widgetMainScroll{
    /* max-height: calc(100vh - 182px);
    overflow-y: scroll;
    overflow-x: hidden;
    scroll-behavior: smooth; */
}
.widgetMainScroll::-webkit-scrollbar-track
{
	-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
	background-color: #F5F5F5;
}

.widgetMainScroll::-webkit-scrollbar
{
	width: 6px;
	background-color: #F5F5F5;
}

.widgetMainScroll::-webkit-scrollbar-thumb
{
	background-color: #000000;
}
.information-box {
  border: 0.5px solid #dadce0;
  border-radius: 4px;
  padding: 0 40px 24px 40px;
}
.back-btn {
  min-height: 33px;
}
.activity-main .form-box {
  display: flex;
  align-items: center;
}
.activity-main .form-box input {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  color: #7d7d7d;
  border: 1px solid #e5e9ee;
  box-sizing: border-box;
  border-radius: 4px;
  height: 50px;
  width: 260px;
  padding: 0 19px;
}
.activity-main .form-box button {
  border: none;
  background: none;
}
.activity-main .form-box button span {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  color: #7d7d7d;
}
.activity-main .form-box .sort-box {
  margin-left: 11px;
}
.activity-box h4 {
  margin-bottom: 35px;
  padding-top: 33px;
  position: sticky;
  top: 0;
}
.vigets-list {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 27px;
}
.vigets-list h4 {
  margin: 0;
}
</style>

