<template>
  <div>
    <Header />
    <Tasklistwidget/>
    <Tasklisttable />
    <Pagination />
  </div>
</template>
<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap");
body {
  font-family: Roboto;
}
.blue-btn {
  transition: all 0.6s;
  background: #4489fe;
}
.blue-btn {
  width: 200px;
  height: 44px;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
}
.blue-btn:hover {
  color: #7d7d7d;
  background: none;
  border: 1px solid #dee0e4;
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

.change-color-a > a {
  color: #212121 !important;
}
</style>
