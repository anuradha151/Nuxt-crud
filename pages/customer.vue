<template>
  <div>
    <div class="box">
      <div class="field">
        <label class="label">Name</label>
        <div class="control">
          <input class="input" v-model="name" type="text" placeholder="e.g Alex Smith">
        </div>
      </div>
      <div class="field">
        <label class="label">Address</label>
        <div class="control">
          <input class="input" v-model="address" type="text" placeholder="e.g Galle">
        </div>
      </div>
      <div class="field">
        <label class="label">Email</label>
        <div class="control">
          <input class="input" id="txtEmail" type="text" placeholder="e.g. alexsmith@gmail.com">
        </div>
      </div>
      <div class="field is-horizontal">
        <div class="field-body">
          <div class="field">
            <label class="label">N.I.C</label>
            <div class="control">
              <input class="input" id="txtNic" type="text" placeholder="e.g 951561630v">
            </div>
          </div>
          <div class="field">
            <label class="label">Passport ID</label>
            <div class="control">
              <input class="input" id="txtPassportId" type="text" placeholder="e.g 11421414124">
            </div>
          </div>
        </div>
      </div>
      <div class="field is-grouped is-grouped-right">
        <p class="control">
          <a v-on:click="save('Hai Anuradha')" id="btnSave" class="button is-primary">
            Submit
          </a>
        </p>
        <p class="control">
          <a class="button is-light">
            Cancel
          </a>
        </p>
      </div>
    </div>
    <div class="reload-button">
      <a class="button is-success">
        <span class="icon is-small">
          <font-awesome-icon icon="circle"></font-awesome-icon>
        </span>
        <span>Reload</span>
      </a>
    </div>
    <div class="customer-table">
      <table class="table is-bordered is-fullwidth is-hoverable">
        <thead>
        <tr>
          <th>Customer ID</th>
          <th>Name</th>
          <th>Address</th>
          <th>E-mail</th>
          <th>N.I.C</th>
          <th>Passport ID</th>
        </tr>
        </thead>
        <tbody>
        <tr v-for="(customer, index) in customers" :key="index">
          <td>{{ customer.id }}</td>
          <td>{{ customer.name }}</td>
          <td>{{ customer.email }}</td>
          <td>{{ customer.address }}</td>
          <td>{{ customer.nic }}</td>
          <td>{{ customer.passport }}</td>
        </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'customer',
    layout: 'cms',

    async asyncData({ app }) {
      let customers = await app.$axios.$get('http://localhost:8081/api/car/customer')
      return {
        customers
      }
    },

    data() {
      return {
        errors: [],
        name: '',
        address: ''
      }
    },
    methods: {
      save: function(message) {
        alert(message)
      },
      reload: function() {

      }
    }
  }

</script>

<style scoped>
  .box {
    margin-right: 1rem;
    width: 50%;

  }
</style>
