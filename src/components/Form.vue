<template>
  <div class="row">
    <div class="mb-3 col-md-6">
      <label class="form-label">Title</label>
      <input type="text" class="form-control addTitle" aria-describedby="" />
    </div>


    <div class="mb-3 col-md-6">
      <label class="form-label">Date</label>
      <input type="date" class="form-control addDate" aria-describedby="" />
    </div>

    <div class="mb-3 col-md-6">
      <label class="form-label">Value</label>
      <input type="number" class="form-control addValue" aria-describedby="" />
    </div>
    <div class="mb-3 col-md-6">
      <label for="title" class="form-label">Description</label>
      <input
        type="text"
        class="form-control addDescrption"
        aria-describedby=""
      />
    </div>
    <div class="mb-3 col-md-12 text-right">
      <button type="submit" class="btn btn-primary addBtn">Add</button>
    </div>
  </div>
</template>

<script>
export default {
    name: "ExpenseForm"
};
</script>
