<template>
  <div>
    <div class="activity-main">
      <b-container>
        <div class="user-box">
          <ul class="head main bg-white">
            <li>User name</li>
            <li>Site Name</li>
            <li>Staff</li>
            <li>Action</li>
            <li>Name</li>
            <li><span class="last">Action</span></li>
          </ul>

          <div class="scroll-table">
        <b-row>
          <b-col cols="12" sm="12" class="my-1" :key="index" v-for="(item, index) in paginatedItems">
          <ul>
            <li><strong>{{item.date}} </strong> <strong>{{item.time}}</strong></li>
            <li>{{item.sitename}}</li>
            <li>
              <div class="img">
                <b-img :src="item.userUrl" /><strong
                  >{{item.staffname}}
                  <p>{{item.staffdesi}}</p></strong
                >
              </div>
            </li>
            <li>{{item.action}}</li>
            <li><a href="#">{{item.name}}</a></li>
            <li>
              <span class="last">
                <b-dropdown
                  id="dropdown-offset"
                  offset="25"
                  text="..."
                  class="m-2 dropdown-box"
                >
                  
                  <b-dropdown-item href="#">Another action</b-dropdown-item>
                  <b-dropdown-item href="#"
                    >Something else here</b-dropdown-item
                  >
                </b-dropdown>
              </span>
            </li>
          </ul>

          </b-col>
        </b-row>


        <b-row>
          <b-col md="12" class="my-1">
            <b-pagination
              align="center"
              @change="onPageChanged"
              :total-rows="totalRows"
              :per-page="perPage"
              v-model="currentPage"
              class="pagination"
              first-text=""
              last-text=""
              first-class="d-none"
              last-class="d-none"
              page-class="border-0"
              active-class="pagination_active"
              exact-active-class="kazim"
            />
          </b-col>
        </b-row>

          <!-- <ul>
            <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>
            <li>France Transcription</li>
            <li>
              <div class="img">
                <b-img src="/_nuxt/assets/i/boy.svg" /><strong
                  >Serhii Movchan
                  <p>Manager</p></strong
                >
              </div>
            </li>
            <li>Add New File</li>
            <li><a href="#">Logo.png</a></li>
            <li>
              <span class="last">
                <b-dropdown
                  id="dropdown-offset"
                  offset="25"
                  text="..."
                  class="m-2 dropdown-box"
                >
                  
                  <b-dropdown-item href="#">Another action</b-dropdown-item>
                  <b-dropdown-item href="#"
                    >Something else here</b-dropdown-item
                  >
                </b-dropdown>
              </span>
            </li>
          </ul>

          <ul>
            <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>
            <li>Ukrainian Transcription</li>
            <li>
              <div class="img">
                <b-img src="/_nuxt/assets/i/boy.svg" /><strong
                  >Vlad Sklyar
                  <p>Transletor</p></strong
                >
              </div>
            </li>
            <li>Create New Page</li>
            <li><a href="#">About Us</a></li>
            <li>
              <span class="last">
                <b-dropdown
                  id="dropdown-offset"
                  offset="25"
                  text="..."
                  class="m-2 dropdown-box"
                >
                  
                  <b-dropdown-item href="#">Another action</b-dropdown-item>
                  <b-dropdown-item href="#"
                    >Something else here</b-dropdown-item
                  >
                </b-dropdown>
              </span>
            </li>
          </ul>

          <ul>
            <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>
            <li>France Transcription</li>
            <li>
              <div class="img">
                <b-img src="/_nuxt/assets/i/boy.svg" /><strong
                  >Serhii Movchan
                  <p>Manager</p></strong
                >
              </div>
            </li>
            <li>Add New File</li>
            <li><a href="#">Logo.png</a></li>
            <li>
              <span class="last">
                <b-dropdown
                  id="dropdown-offset"
                  offset="25"
                  text="..."
                  class="m-2 dropdown-box"
                >
                  
                  <b-dropdown-item href="#">Another action</b-dropdown-item>
                  <b-dropdown-item href="#"
                    >Something else here</b-dropdown-item
                  >
                </b-dropdown>
              </span>
            </li>
          </ul>

          <ul>
            <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>
            <li>Ukrainian Transcription</li>
            <li>
              <div class="img">
                <b-img src="/_nuxt/assets/i/boy.svg" /><strong
                  >Vlad Sklyar
                  <p>Transletor</p></strong
                >
              </div>
            </li>
            <li>Create New Page</li>
            <li><a href="#">About Us</a></li>
            <li>
              <span class="last">
                <b-dropdown
                  id="dropdown-offset"
                  offset="25"
                  text="..."
                  class="m-2 dropdown-box"
                >
                  
                  <b-dropdown-item href="#">Another action</b-dropdown-item>
                  <b-dropdown-item href="#"
                    >Something else here</b-dropdown-item
                  >
                </b-dropdown>
              </span>
            </li>
          </ul>

          <ul>
            <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>
            <li>France Transcription</li>
            <li>
              <div class="img">
                <b-img src="/_nuxt/assets/i/boy.svg" /><strong
                  >Serhii Movchan
                  <p>Manager</p></strong
                >
              </div>
            </li>
            <li>Add New File</li>
            <li><a href="#">Logo.png</a></li>
            <li>
              <span class="last">
                <b-dropdown
                  id="dropdown-offset"
                  offset="25"
                  text="..."
                  class="m-2 dropdown-box"
                >
                  
                  <b-dropdown-item href="#">Another action</b-dropdown-item>
                  <b-dropdown-item href="#"
                    >Something else here</b-dropdown-item
                  >
                </b-dropdown>
              </span>
            </li>
          </ul>
          <ul>
            <li><strong>25/06/2020 </strong> <strong>04:55 PM</strong></li>
            <li>Ukrainian Transcription</li>
            <li>
              <div class="img">
                <b-img src="/_nuxt/assets/i/boy.svg" /><strong
                  >Vlad Sklyar
                  <p>Transletor</p></strong
                >
              </div>
            </li>
            <li>Create New Page</li>
            <li><a href="#">About Us</a></li>
            <li>
              <span class="last">
                <b-dropdown
                  id="dropdown-offset"
                  offset="25"
                  text="..."
                  class="m-2 dropdown-box"
                >
                  
                  <b-dropdown-item href="#">Another action</b-dropdown-item>
                  <b-dropdown-item href="#"
                    >Something else here</b-dropdown-item
                  >
                </b-dropdown>
              </span>
            </li>
          </ul> -->
        </div>
        </div>

      </b-container>
    </div>
  </div>
</template>


<script>
const items = [
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "English Transcription 1",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "David Jonas",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "English Transcription 2",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "David Jonas",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "English Transcription 3",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "David Jonas",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "English Transcription 4",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "David Jonas",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "English Transcription 5",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "David Jonas",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "Second Page 6",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Shoaib Javed",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "Second Page  7",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Shoaib Javed",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "Second Page  Transcription 8",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Shoaib Javed",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "Second Page  Transcription 8",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Shoaib Javed",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "Second Page  Transcription 10",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Shoaib Javed",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "Third Page  11",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Kazim Ali",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "Third Page",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Kazim Ali",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "Third Page",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Kazim Ali",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "Third Page",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Kazim Ali",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020 4",
     time: "04:55 PM",
     sitename: "Third Page",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Kazim Ali",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020 5",
     time: "04:55 PM",
     sitename: "Forth Page Transcription",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Rana Qasim",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "Forth Page  Transcription 8",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Rana Qasim",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020 last",
     time: "04:55 PM",
     sitename: "Forth Page  Transcription 8",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Rana Qasim",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  }, {
     date: "25/06/2020",
     time: "04:55 PM",
     sitename: "Forth Page  Transcription 8",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Rana Qasim",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  },
  {
     date: "25/06/2020 last",
     time: "04:55 PM",
     sitename: "Forth Page  Transcription 8",
     userUrl: "/_nuxt/assets/i/boy.svg",
     staffname: "Rana Qasim",
     staffdesi: "Manager",
    action: "Create New Task",
    name: "ulanscription"
  }
];

export default {
  name: "MyBootstrapGrid",
  data() {
    return {
      items: items,
      paginatedItems: items,
      currentPage: 1,
      perPage: 5,
      totalRows: items.length
    };
  },
  computed: {},
  methods: {
    paginate(page_size, page_number) {
      let itemsToParse = this.items;
      this.paginatedItems = itemsToParse.slice(
        page_number * page_size,
        (page_number + 1) * page_size
      );
    },
    onPageChanged(page) {
      this.paginate(this.perPage, page - 1);
    }
  },
  mounted() {
    this.paginate(this.perPage, 0);
  }
};
</script>

<style scoped>
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
.user-box ul li:nth-child(1) {
  max-width: 130px;
}
.user-box ul li:nth-child(2) {
 max-width: 230px;
}
.user-box ul li:nth-child(3) {
  max-width: 260px;
}
.user-box ul li:nth-child(4) {
  max-width: 290px;
}
.user-box ul li:nth-child(5) {
  max-width: 290px;
}
.user-box ul li:nth-child(6) {
  max-width: 30px;
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



</style>

