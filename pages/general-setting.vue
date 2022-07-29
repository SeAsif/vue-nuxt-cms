<template>
  <div id="scrollStyle3" class="">
    <Header />
    <div class="container-100">
    <Nikepronav />
    <b-container>
    <b-row class="no-gutters">
      <b-col lg="5">
        <b-row class=" margin-0">
          <b-col col="6" md="6" lg="6" class="p-0">
            <Searchbar />
            <Directory />
          </b-col>

          <b-col col="6" md="6" lg="6" class="pl-0">
            <Generalsettings/>
          </b-col>
        </b-row>
      </b-col>

      <b-col lg="7"><Generalform /></b-col>
      <Newpagemodel />
    </b-row>
</b-container>
</div>
  </div>
</template>
