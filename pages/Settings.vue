<template>
  <div id="scrollStyle3">
    <Header />
    <b-container class="mt-5 pt-1">
      <div>
        <b-tabs
          nav-class="setting-sidebar"
          content-class="mainTabs"
          class="sidebar-main"
          vertical
        >
          <b-tab>
            <template class="h3-first" #title>
              <div class="hover-switch">
                <h3 class="setting-h3">Settings</h3>
              </div>
            </template>
          </b-tab>

          <b-tab active>
            <template #title>
              <div class="hover-switch">
                <div class="icon">
                  <img src="~assets/i/setting-grey.svg" />
                  <img src="~assets/i/setting.svg" />
                </div>
                <div class="text">
                  <h4>General</h4>
                  <p>General Site Settings</p>
                </div>
              </div>
            </template>
            <div><Generalinformation /></div>
          </b-tab>

          <b-tab>
            <template #title>
              <div class="hover-switch">
                <div class="icon">
                  <img src="~assets/i/vigeets.svg" />
                  <img src="~assets/i/vigeets2.svg" class="one" />
                </div>
                <div class="text">
                  <h4>Widgets</h4>
                  <p>Widgets Settings</p>
                </div>
              </div>
            </template>
            <div><Vigetslist /></div>
          </b-tab>

          <b-tab>
            <template #title>
              <div class="hover-switch">
                <div class="icon">
                  <img src="~assets/i/pages.svg" alt="" />
                  <img src="~assets/i/pages2.svg" class="two" alt="" />
                </div>
                <div class="text">
                  <h4>Page Types</h4>
                  <p>Page Type Settings</p>
                </div>
              </div>
            </template>
            <div><Typelist /></div>
          </b-tab>
        </b-tabs>
      </div>

      <b-row>
        <b-col lg="3">
          <!-- <Settingssidebar /> -->
        </b-col>
        <b-col lg="9"> </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<style scoped>
.mainTabs {
}
</style>
