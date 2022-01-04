<template>
  <tr>
    <td><input type="checkBox" /></td>
    <td>{{ slno }}</td>
    <td>Honda</td>
    <td>City</td>
    <td>2015</td>
    <td>Sedan</td>
    <td>UVA</td>
    <td>Bumper</td>
    <td>123456</td>
    <td>4500.00</td>
    <td>5300.00</td>
    <td>8</td>
    <td>8 Days</td>
    <td>
      <button
        class="btn btn-outline-primary"
        style="border-color: #194a82; color: #194a82; margin-right: 10px"
      >
        Reject
      </button>
      <button class="btn bg-theme-pr">Approve</button>
    </td>
  </tr>
</template>

<script>
export default {
  name: "TableRow",
  props: ["slno"],
};
</script>

<style scoped>
.bg-theme-pr {
  background-color: #194a82;
  color: white;
}
td:not(:last-child) {
  padding-top: 15px !important;
}
</style>