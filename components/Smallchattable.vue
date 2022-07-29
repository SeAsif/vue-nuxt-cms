<template>
  <div>
    <div class="activity-main border-right">
      <div class="user-box last pr-0">
        <ul class="head">
          <li>Task Name</li>
          <li>Creation Date</li>
          <li>Staff</li>
          <li>Pages in Project</li>
        </ul>
        <ul>
          <li>English Transcription</li>
          <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>

          <li>
            <div class="img img-absolute">
              <b-img src="~/assets/i/boy.svg" />
              <b-img src="~/assets/i/boy.svg" />
              <b-img src="~/assets/i/boy.svg" />
              <b-img src="~/assets/i/boy.svg" />
            </div>
          </li>
          <li><a href="#">View</a></li>
        </ul>
        <ul>
          <li>France Transcription</li>
          <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>

          <li>
            <div class="img">
              <b-img src="~/assets/i/boy.svg" /><strong
                >Serhii Movchan
                <p>Manager</p></strong
              >
            </div>
          </li>
          <li><a href="#">View</a></li>
        </ul>

        <ul>
          <li>Ukrainian Transcription</li>
          <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>

          <li>
            <div class="img">
              <b-img src="~/assets/i/boy.svg" /><strong
                >Serhii Movchan
                <p>Manager</p></strong
              >
            </div>
          </li>
          <li><a href="#">View</a></li>
        </ul>
        <ul>
          <li>Russion Transcription</li>
          <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>

          <li>
            <div class="img">
              <b-img src="~/assets/i/boy.svg" /><strong
                >Serhii Movchan
                <p>Manager</p></strong
              >
            </div>
          </li>
          <li><a href="#">View</a></li>
        </ul>

        <ul>
          <li>English Transcription</li>
          <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>

          <li>
            <div class="img img-absolute">
              <b-img src="~/assets/i/boy.svg" />
              <b-img src="~/assets/i/boy.svg" />
              <b-img src="~/assets/i/boy.svg" />
              <b-img src="~/assets/i/boy.svg" />
            </div>
          </li>
          <li><a href="#">View</a></li>
        </ul>

        <ul>
          <li>France Transcription</li>
          <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>

          <li>
            <div class="img">
              <b-img src="~/assets/i/boy.svg" /><strong
                >Serhii Movchan
                <p>Manager</p></strong
              >
            </div>
          </li>
          <li><a href="#">View</a></li>
        </ul>
        <ul>
          <li>Ukrainian Transcription</li>
          <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>

          <li>
            <div class="img">
              <b-img src="~/assets/i/boy.svg" /><strong
                >Serhii Movchan
                <p>Manager</p></strong
              >
            </div>
          </li>
          <li><a href="#">View</a></li>
        </ul>

        <ul>
          <li>Russion Transcription</li>
          <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>

          <li>
            <div class="img">
              <b-img src="~/assets/i/boy.svg" /><strong
                >Serhii Movchan
                <p>Manager</p></strong
              >
            </div>
          </li>
          <li><a href="#">View</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>
<style scoped>
.user-box.last ul li:last-child {
    width: 55%;
}
.activity-main.border-right .user-box ul {
  border-right: 0;
}
.user-box {
  padding: 0 30px;
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
.user-box ul {
  display: flex;
  width: 100%;
  margin: 0;
  border: 1px solid #e5e9ee;
  border-radius: 4px;
  padding: 0 31px;
  min-height: 80px;
  align-items: center;
  margin-bottom: 8px;
}
.user-box ul.head li {
  font-style: normal;
  font-weight: 500;
  font-size: 12px;
  color: #212121;
}
.user-box ul li {
  width: 100%;
  list-style-type: none;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  color: #212121;
}
.user-box ul li span {
  display: flex;
  justify-content: flex-end;
}
.user-box ul li .img {
  display: flex;
  align-items: center;
}
strong p {
  margin: 0;
  color: #7d7d7d;
}
.user-box ul li .img strong {
  margin-left: 9px;
}
li.last {
  text-align: end !important;
}
.user-box ul li a {
  color: #4489fe;
}
.user-box ul li span.last {
  text-align: end;
}
.user-box ul li strong {
  font-weight: 400;
  display: block;
}
.user-box ul.head {
  border: none;
  min-height: 45px;
  margin: 0;
  padding: 31px 31px 14px;
}
.user-box .img-absolute img {
  margin: 0 -19px 0 0;
  width: 40px;
  height: 40px;
}
</style>
