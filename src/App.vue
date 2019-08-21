<template>
  <div id="app" class="small-container">
    <h1>Employees</h1>

    <employee-table :employees="employees"/>
  </div>
</template>

<script>
import EmployeeTable from '@/components/EmployeeTable.vue'

export default {
  name: 'app',
  components: {
    EmployeeTable,
  },
  data() {
    return {
      employees: [
        {
          id: 1,
          name: 'You suck Hendricks',
          email: 'richard@piedpiper.com',
        },
        {
          id: 2,
          name: 'Bertram rules!',
          email: 'gilfoyle@piedpiper.com',
        },
        {
          id: 3,
          name: 'Dinesh Chugtai',
          email: 'dinesh@piedpiper.com',
        },
        {
          id: 4,
          name: 'Yoga Bear',
          email: 'dinesh@piedpiper.com',
        },
      ],
    }
  },
}
  
</script>

<style>
  button {
    background: #009435;
    border: 1px solid #009435;
  }

  .small-container {
    max-width: 680px;
  }
</style>