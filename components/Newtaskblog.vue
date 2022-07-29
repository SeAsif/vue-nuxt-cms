<template>
    <div>
        
<div class="banner-blog">
   
       <b-row>
           <b-col lg="6" class="pr-4">

 <div class="position-relative mb--4 mt-3 input-style">
            <b-form-input type="text" placeholder="Select and click on button for add staff" id=""></b-form-input>
          </div>
   
   
    <div class="blog-checkbox bg-img">
    
    <b-form-checkbox
      id="checkbox-2"
      v-model="status"
      name="checkbox-2"
      value="accepted"
      unchecked-value="not_accepted"
    >
    <b-img src="~assets/i/boy.svg" alt="" />
     <span> Serhii Movchan</span>
    </b-form-checkbox>

<b-form-checkbox
      id="checkbox-3"
      v-model="status"
      name="checkbox-3"
      value="accepted"
      unchecked-value="not_accepted"
    >
    <b-img src="~assets/i/boy-1.svg" alt="" />
      <span>Artem Reznichkov</span>
    </b-form-checkbox>
    <b-form-checkbox
      id="checkbox-4"
      v-model="status"
      name="checkbox-4"
      value="accepted"
      unchecked-value="not_accepted"
    >
    <b-img src="~assets/i/boy-2.svg" alt="" />
      <span>Vlad Sklyar</span>
    </b-form-checkbox>
      <b-form-checkbox
      id="checkbox-5"
      v-model="status"
      name="checkbox-5"
      value="accepted"
      unchecked-value="not_accepted"
    >
    <b-img src="~assets/i/boy-3.svg" alt="" />
      <span>Vasilii Kovalchuk</span>
    </b-form-checkbox>
      <b-form-checkbox
      id="checkbox-6"
      v-model="status"
      name="checkbox-6"
      value="accepted"
      unchecked-value="not_accepted"
    >
    <b-img src="~assets/i/boy-4.svg" alt="" />
      <span>Dima Steetsyna</span>
    </b-form-checkbox>
      <b-form-checkbox
      id="checkbox-7"
      v-model="status"
      name="checkbox-7"
      value="accepted"
      unchecked-value="not_accepted"
    >
    <b-img src="~assets/i/boy-5.svg" alt="" />
     <span> John Doe</span>
    </b-form-checkbox>
      
</div>
</b-col>
 <b-col lg="6" class="pl-4">

 <div class="position-relative mb--4 mt-3 input-style">
            <b-form-input type="text" placeholder="Select and click on button for remove staff
" id=""></b-form-input>
          </div>
   
   
    <div class="blog-checkbox">
   
    <b-form-checkbox
      id="checkbox-10"
      v-model="status"
      name="checkbox-10"
      value="accepted"
      unchecked-value="not_accepted"
    >
    <b-img src="~assets/i/boy-6.svg" alt="" />
     <span> Serhii Godym</span>
    </b-form-checkbox>

<b-form-checkbox
      id="checkbox-11"
      v-model="status"
      name="checkbox-11"
      value="accepted"
      unchecked-value="not_accepted"
    >
    <b-img src="~assets/i/boy-7.svg" alt="" />
      <span>Max Kashchenko</span>
    </b-form-checkbox>
    <b-form-checkbox
      id="checkbox-12"
      v-model="status"
      name="checkbox-12"
      value="accepted"
      unchecked-value="not_accepted"
    >
    <b-img src="~assets/i/boy-8.svg" alt="" />
      <span>Max Schutskii</span>
    </b-form-checkbox>
     
    
</div>

</b-col>

 </b-row> 
  

</div>

    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
.blog-input .position-relative{
    width: 40%;
}
.input-style input{    color: #7D7D7D;
    font-size: 14px;
    font-weight: 400;
    line-height: 16px;
        height: 50px;}
.blog-checkbox {
    border: 1px solid #DEE0E4;
    padding: 0;
        height: 290px;
    overflow-y: scroll;
    margin: 20px 0 0 0;
    border-radius: 4px;
    }

.blog-checkbox custon-checkbox {
    padding: 40px 0;
}

.blog-checkbox .custom-checkbox {
   padding: 9px 0 9px 43px;
    text-align: left;
    cursor: pointer;
}
.blog-checkbox::-webkit-scrollbar {
  display: none;
}
.blog-checkbox .custom-checkbox:hover{
    background-color: #E9F0FD;
}
.blog-checkbox {
  /* -ms-overflow-style: none; 
  scrollbar-width: none;   */
}
.blog-checkbox .custom-control-label span{
    position: relative;
    margin-bottom: 0;
    vertical-align: top;
    font-size: 14px;
    color: #212121;
    padding: 0 0 0 4px;
        line-height: 27px;
}
.blog-checkbox .custom-control-label img{
        height: 30px;
    padding:0 0 0 4px;
}
.bg-img::before{content: ""; background-image: url("~assets/i/fill-arrow-next.svg");
     content: "";
    background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyMiAyMiIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0xNS40MjAzIDIxLjgzMzNMNi41Njk0OSAyMS44MzMzQzIuNzQ1MzMgMjEuODMzMyAwLjE2Njk5MiAxOS4zNzMxIDAuMTY2OTkyIDE1LjcwMTdMMC4xNjY5OTIgNi4zMDkxNkMwLjE2Njk5MiAyLjYzNjY2IDIuNzQ1MzMgMC4xNjY2NTYgNi41Njk0OSAwLjE2NjY1NkwxNS40MjAzIDAuMTY2NjU2QzE5LjI1NTMgMC4xNjY2NTYgMjEuODMzNyAyLjYzNjY2IDIxLjgzMzcgNi4zMDkxNkwyMS44MzM3IDE1LjcwMTdDMjEuODMzNyAxOS4zNzMxIDE5LjI1NTMgMjEuODMzMyAxNS40MjAzIDIxLjgzMzNaTTEzLjQ1OTUgMTAuMTg3NUg2LjU4MDMzQzYuMTI1MzMgMTAuMTg3NSA1Ljc2NzgzIDEwLjU1NTggNS43Njc4MyAxMUM1Ljc2NzgzIDExLjQ1NSA2LjEyNTMzIDExLjgxMjUgNi41ODAzMyAxMS44MTI1SDEzLjQ1OTVMMTAuNzcyOCAxNC40ODgzQzEwLjYyMTIgMTQuNjQgMTAuNTM0NSAxNC44NTY3IDEwLjUzNDUgMTUuMDYyNUMxMC41MzQ1IDE1LjI2NzIgMTAuNjIxMiAxNS40NzQyIDEwLjc3MjggMTUuNjM2N0MxMS4wODcgMTUuOTUwOCAxMS42MDcgMTUuOTUwOCAxMS45MjEyIDE1LjYzNjdMMTYuMDA1MyAxMS41NzQyQzE2LjMwODcgMTEuMjcwOCAxNi4zMDg3IDEwLjcyOTIgMTYuMDA1MyAxMC40MjU4TDExLjkyMTIgNi4zNjMzMkMxMS42MDcgNi4wNDkxNiAxMS4wODcgNi4wNDkxNiAxMC43NzI4IDYuMzYzMzJDMTAuNDU4NyA2LjY4ODMyIDEwLjQ1ODcgNy4xOTc0OSAxMC43NzI4IDcuNTIyNDlMMTMuNDU5NSAxMC4xODc1WiIgZmlsbD0iIzQ0ODlGRSIvPgo8L3N2Zz4K);
    position: absolute;
    right: 0;
    top: 50%;
    transform: translate(11px, 232%);
    width: 22px;
    height: 22px;
    background-repeat: no-repeat;
    cursor: pointer;
    }
    .bg-img::after{content: ""; background-image: url("~assets/i/fill-arrow-back.svg");
 position: absolute;
    right: 0;
   top: 50%;
       transform: translate(10px, 80%);
    width: 22px;
    height: 22px;
    background-repeat: no-repeat;
    cursor: pointer;
    }
  
</style>