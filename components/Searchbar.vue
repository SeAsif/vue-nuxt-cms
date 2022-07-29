<template>
  <div>
    <b-container fluid>
      <div class="search-box">
        <b-img src="~assets/i/search-icon.svg" alt="" />
        <b-form-input
          size="sm"
          class="mr-sm-2"
          placeholder="Search"
        ></b-form-input>
        <div class="search-images">
          <b-link rel="stylesheet" to="/"><b-img src="~assets/i/paper-plus.svg" alt="" /></b-link>
          <b-link rel="stylesheet" to="/"> <b-img src="~assets/i/folder-plus.svg" alt="" /></b-link>
        </div>
      </div>
    </b-container>
  </div>
</template>  

<style scoped>
.search-box {
  position: relative;
  display: flex;
  align-items: center;
  padding: 0 0 10px 0;
  border-bottom: 1px solid #e5e9ee;
  margin: 10px 0 0 0;
}

.search-box input {
  border: 0px;
  padding: 0 53px 0 34px;
  font-size: 14px;
  font-family: "Roboto";
  font-weight: 400;
  line-height: 20px;
  margin: 3px 0 0 0;
}

.search-box img {
  position: absolute;
  top: 10px;
  bottom: 0;
  width: 17px;
  height: 17px;
  left: 4px;
}

.search-images img {
  position: inherit;
  margin: 0 5px;
  width: 17px;
  height: 17px;
}

.search-images {
  position: absolute;
  top: 7px;
  right: 0;
}
.form-control:focus {
  box-shadow: none;
}
</style>