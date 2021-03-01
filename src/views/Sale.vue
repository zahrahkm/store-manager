<template>
  <div class="sale">
    <div class="container">
      <form autocomplete="off">
        <div class="form-control">
          <label>Search product</label>
          <input type="text" name="text" placeholder="Search..." />
        </div>
        <div class="num-btn">
          <input type="number" name="number" placeholder="No." />
          <button type="submit">Add</button>
        </div>
      </form>
      <table>
        <tr>
          <th>#</th>
          <th>Product</th>
          <th>No.</th>
          <th>Price</th>
          <th>Total</th>
        </tr>
        <tr>
          <td>
            1
          </td>
          <td>
            Basket
          </td>
          <td>
            3
          </td>
          <td>
            5.50
          </td>
          <td>
            16.50
          </td>
        </tr>
        <tr>
          <td>
            2
          </td>
          <td>
            Pan
          </td>
          <td>
            2
          </td>
          <td>
            9.50
          </td>
          <td>
            19
          </td>
        </tr>
        <tr>
          <td>-</td>
          <td><strong>Total</strong></td>
          <td><strong>5</strong></td>
          <td>-</td>
          <td><strong>35.50</strong></td>
        </tr>
      </table>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Sale",
  components: {}
});
</script>

<style scoped>
.sale {
  background-color: #fdba74;
  min-height: 100vh;
  padding: 1rem;
}
.container {
  background-color: white;
  width: 100%;
  margin: auto;
  padding: 1rem;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.25);
}
form {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  margin: auto;
  width: 90%;
}
.form-control {
  display: flex;
  flex-direction: column;
}
.form-control label {
  margin-bottom: 0.3rem;
}
.num-btn {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
form input {
  margin-bottom: 1rem;
  padding: 6px;
  border: none;
  border: 1px solid rgba(125, 45, 18, 0.5);
}
form input:focus {
  outline: none;
  border: 1px solid #7c2d12;
}
form input[type="number"] {
  width: 60px;
}
form button {
  margin-bottom: 1rem;
  width: 50%;
  padding: 6px;
  border: 1px solid #fdba74;
  background-color: #fdba74;
}
table,
th,
td {
  border: 1px solid rgba(125, 45, 18, 0.5);
  border-collapse: collapse;
  padding: 4px;
  text-align: left;
}
table {
  width: 90%;
  margin: 1rem auto;
}
tr {
  font-size: small;
}
tr:last-child {
  background-color: rgba(253, 187, 116, 0.2);
}
</style>
