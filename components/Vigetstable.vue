<template>
  <div>
    <div class="activity-main">
      <div class="user-box">
        <ul class="head bg-white">
          <li>Name</li>
          <li>Last Activite</li>
          <li>Action</li>
          <li><span class="last">Action</span></li>
        </ul>

      <div class="scroll-table">
        <b-row>
          <b-col cols="12" sm="12" class="my-1" :key="index" v-for="(item, index) in paginatedItems">

            <ul>
              <li>{{item.name}}</li>
              <li><strong>{{item.activitedate}} </strong> <strong>{{item.activitetime}}</strong></li>
              <li>{{item.action}}</li>
              <li>
                <span class="last">
                  <b-dropdown
                    id="dropdown-offset"
                    offset="25"
                    text="..."
                    class="m-2 dropdown-box"
                  >
                    
                    <b-dropdown-item href="#">Another action</b-dropdown-item>
                    <b-dropdown-item href="#">Something else here</b-dropdown-item>
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

        </div>
      </div>
    </div>
  </div>
</template>

<script>
const items = [
  {
     name: "Blog Widget 1 Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Blog Widget 1 Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Blog Widget 1 Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Blog Widget 1 Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Blog Widget 1 Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 2 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 2 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 2 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 2 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 2 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 3 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 3 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 3 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 3 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 3 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 4 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 4 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 4 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 4 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  },
  {
     name: "Page 4 of Data",
     activitedate: "25/06/2020",
     activitetime: "04:55 PM",
     action: "Add New widget"

  }

];

export default {
  scrollToTop: true,
  name: "MyBootstrapGrid",
  data() {
    return {
      items: items,
      paginatedItems: items,
      currentPage: 1,
      perPage: 3,
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

      const chatLogDiv = document.getElementById('scrolltopm')
      chatLogDiv.scrollTop = 0


      console.log("OK pagination")
    },
    handleClick(page) {
     const chatLogDiv = document.getElementById('scrolltopm')
      chatLogDiv.scrollTop = 0
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
  padding: 14px 31px 14px;
    z-index: 1040;
}
</style>

