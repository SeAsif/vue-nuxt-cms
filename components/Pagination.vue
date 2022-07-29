<template>
  <div>
    <div class="mt-3">
      <ul class="pagination">
        <li>
          <a href="#"><b-img src="~assets/i/back-btn.svg"/></a>
        </li>
        <li><a href="#" class="active">1</a></li>
        <li><a href="#">2</a></li>
        <li><a href="#">3</a></li>
        <li><a href="#">4</a></li>
        <li><a href="#">5</a></li>
        <li><a href="#">6</a></li>
        <li><a href="#">...</a></li>
        <li><a href="#">14</a></li>
        <li><a href="#">15</a></li>
        <li>
          <a href="#"><b-img src="~assets/i/right-arrow.svg"/></a>
        </li>
      </ul>
    </div>
  </div>
</template>
<style>
.pagination li a {
  padding: 6px 11px;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  color: #212121;
}
.pagination li a.active{
  border-left: 0px solid #4489fe !important;
}
ul.pagination li a:hover {
  border-left: none !important;
  background-color: transparent;
}
.pagination li a.active {
  background-color: #4489fe !important;
  border-radius: 4px;
  color: #fff;
}
.pagination {
  justify-content: center;
  padding: 58px 0 30px;
  align-items: center;
}
</style>
