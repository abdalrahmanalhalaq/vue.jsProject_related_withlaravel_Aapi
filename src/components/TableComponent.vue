<template>
     <div class="row mt-5 mb-5">
      <div class="custom-card ">
        <table class="table ">
          <thead>
            <tr>
              <th> #</th>
              <th> Title</th>
              <th> Date</th>
              <th>value</th>
              <th>Description</th>
              <th></th>
            </tr>
          </thead>
          <tbody>
            <row-component v-for="(item) in expenses" :key="item.id" :expense="item" :delete-row="deleteRow"></row-component>
          </tbody>
        </table>
        <!-- #cusotm card -->
      </div>
    </div>
</template>

<script>
import RowComponent from './RowComponent.vue';

export default {
  components: {
    RowComponent
  },
  data() {
      return {
        expenses: [
          {id: 1, title: "T1", date: "2022-05-10", value: "100", description: "Description T1"},
          {id: 2, title: "T2", date: "2022-05-11", value: "200", description: "Description T2"},
          {id: 3, title: "T3", date: "2022-05-12", value: "300", description: "Description T3"},
          {id: 4, title: "T4", date: "2022-05-13", value: "400", description: "Description T4"},
        ],
      };
  },
  methods: {
    deleteRow(event, id) {
      console.log(event);
      console.log(id);
      // alert('Delete Row: '+id);
      this.expenses = this.expenses.filter((item) => item.id != id);
    }
  }
}
</script>