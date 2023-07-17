<template>
    <tr>
      <td> {{ expense.id }} </td>
      <td> {{ expense.title }} </td>
      <td> {{ expense.date }} </td>
      <td> {{expense.value}}$ </td>
      <td colspan="2"> {{ expense.description }} </td>
      <td class="text-right">
        <a class="delete" @click="deleteRow($event, expense.id)">
            <i class="fa fa-trash-o" aria-hidden="true"></i>
        </a>
    </td>
    </tr>
</template>

<script>
export default {
    props: ["expense", "deleteRow"],
    data() {},
    methods: {
        // deleteRow(event, id) {
        //     // event.preventDefault();
        //     console.log(id);
        //     // console.log(event.target.closest('tr').remove());
        //     // event.target.closest('tr').remove();
        //     // event.parent.remove();
        // }
    }
}
</script>