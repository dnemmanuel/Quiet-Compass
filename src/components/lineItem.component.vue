<template>
  <div class="wrapper">
    <table>
    <thead class="blue-grey darken-4">
      <tr>
        <th>Title</th>
        <th>Status</th>
        <th>Due Date</th>
        <th>Assigned By</th>
        <th>Category</th>
      </tr>
    </thead>
    <tbody class="grey darken-4">
      <tr v-for="line in lines" :key="line.id">
        <td>{{ line.title }}</td>
        <td>{{ line.status }}</td>
        <td>{{ line.due_date }}</td>
        <td>{{ line.assigned_by }}</td>
        <td>{{ line.category }}</td>
      </tr>
    </tbody>
  </table>
  </div>
</template>

<script>
import lines from '@/dataSheets/lineData.json'
export default {
  data() {
    return {
      lines
    }
  },
};
</script>

<style lang="css">
.wrapper {
  height: 500px !important;
  overflow-y: scroll;
}
table {
  overflow: hidden;
  border-radius: 8px;
}
td {
  position: sticky;
  top: 0;
}
td,
th {
  padding: 24px;
  margin: 0 !important;
  border-radius: 0 !important;
}

/* width */
::-webkit-scrollbar {
  width: 10px;
}

/* Track */
::-webkit-scrollbar-track {
  background: #f1f1f100;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #888;
  border-radius: 10px;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #555;
}
</style>
