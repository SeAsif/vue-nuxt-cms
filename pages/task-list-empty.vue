<template>
  <div>
<b-container fluid>
    <b-row>
     
      <b-col>
        <Tasklist/>
      </b-col>
  </b-row>
  <b-row>

  
      <b-col lg="12" class="d-flex align-items-lg-center justify-content-center pagesection"><Addtask /></b-col>
  </b-row>
  <Newtaskmodel/> 
  </b-container>
  </div>
</template>

<style scoped>
.pagesection{
    height: calc(100vh - 138px);
}
</style>