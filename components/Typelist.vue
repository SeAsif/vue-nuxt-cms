<template>
  <div>
    <div class="tab-2 d-none" :class="{ active: isActive2 }">
      <div class="back-btn"></div>
      <div class="information-box widgetMainScroll activity-main" id="scrolltopmm">
        <div class="activity-box bg-white">
          <div class="vigets-list pt-4">
            <h4>Page Type List</h4>
            <b-button  v-on:click="craetePage()" variant="primary" class="btn-blue"
              >Add New Page Types</b-button
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
        <Typelisttable />
        <!-- <Pagination/> -->
      </div>
    </div>

      <div class="d-none" :class="{ active: isActive }"><CreatePageType /></div>

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
.active{
  display: block !important;
}
.information-box {
  border: 0.5px solid #dadce0;
  border-radius: 4px;
  padding: 0px 40px;
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
}
.vigets-list {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 27px;
}

</style>



