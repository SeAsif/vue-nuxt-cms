<template>
  <div>
    <div class="activity-main">
      <b-container>
        <div class="activity-box">
          <h4>Activity</h4>
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
      </b-container>
    </div>
  </div>
</template>

<style>
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
</style>
