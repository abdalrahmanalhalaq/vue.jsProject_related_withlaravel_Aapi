<template>
  <div class="container mt-5">
    <!-- row : from -->
    <div class="row">
      <!-- col -->
      <div class="col-sm-6">
        <img src="./assets/images/m1.png" class="img-fluid" alt="" />
      </div>
      <div class="col-sm-6 mt-5">
        <div class="row tit">
          <h4 class="">wellcom to Momen Expense Manager </h4>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            dolore magna aliqua. Ut enim ad minim veniam
          </p>
        </div>
      <expense-form></expense-form>
      </div>
      <!-- #col -->
    </div>
    <!-- #row : from -->
    <table-component></table-component>
    <!-- row :dispaly table -->
   
    <!-- #row :dispaly table -->
  </div>
  </template>

<script>
import ExpenseForm from './components/Form.vue';
import TableComponent from './components/TableComponent.vue';

export default {
  name: 'App',
  components: {
    ExpenseForm,
    TableComponent,
}
}
</script>

<style>

</style>
