<template>
  <div>
   
    <div class="Sections-Yet text-center">
      <h3>You Don’t Have Any Task Yet</h3>
      <p>Please add your first task</p>
      <b-img src="~assets/i/add-new-task.svg" />
         <b-button
        class="btn-blue d-block"
        variant="link"
        id="show-btn"
        @click="$bvModal.show('bv-modal-example')"
        >Add New Task</b-button
      >
 </div>
    </div>
  
</template>

<style scoped>
.Sections-Yet .btn-blue {
  margin: 0 auto;
  width: 251px;
  height: 44px;
}
.Sections-Yet h3 {
  font-weight: normal;
  font-size: 24px;
}
.Sections-Yet p {
  font-weight: normal;
  font-size: 14px;
  color: #7d7d7d;
  margin-bottom: 28px;
}
.Sections-Yet img {
  margin-bottom: 26px;
}
</style>
