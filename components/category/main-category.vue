<template>
  <div class="box">
    <div class="columns">
      <div class="column">
         <span class="icon is-small is-left">
            <font-awesome-icon class="has-text-success" icon="dot-circle"></font-awesome-icon>
        </span>
        <span class="is-size-5">Main Category</span>
      </div>
      <div class="column">
        <a class="button is-danger">
          <span class="icon">
            <font-awesome-icon icon="plus"></font-awesome-icon>
          </span>
          <span>Add Category</span>
        </a>
      </div>
    </div>
    <div>
      <table class="table is-striped is-fullwidth">
        <tr class="row01">
          <td>Test 01</td>
          <td class="col-edit"><a href="#">Edit</a></td>
          <td class="col-delete"><a href="#">Delete</a></td>
        </tr>
        <tr class="row01">
          <td>Test 01</td>
          <td class="col-edit"><a href="#">Edit</a></td>
          <td class="col-delete"><a href="#">Delete</a></td>
        </tr>
        <tr class="row01">
          <td>Test 01</td>
          <td class="col-edit"><a href="#">Edit</a></td>
          <td class="col-delete"><a href="#">Delete</a></td>
        </tr>
        <tr class="row01">
          <td>Test 01</td>
          <td class="col-edit"><a href="#">Edit</a></td>
          <td class="col-delete"><a href="#">Delete</a></td>
        </tr>
        <tr class="row01">
          <td>Test 01</td>
          <td class="col-edit"><a href="#">Edit</a></td>
          <td class="col-delete"><a href="#">Delete</a></td>
        </tr>
      </table>
    </div>
  </div>
</template>
<style scoped>
  .row01 {
    text-align: center;

  }

  .box {
    width: 400px;
  }

  .button {
    padding: 5px;
    margin-left: 40px;
  }

  .col-delete {
    text-align: center;
  }

  .col-edit {
    text-align: center;
  }

</style>
