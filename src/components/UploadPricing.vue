<template>
  <NavBar />
  <div class="container-fluid bg-skyBlue">
    <div class="container">
      <nav aria-label="breadcrumb">
        <ol class="breadcrumb">
          <li class="breadcrumb-item">
            <a href="#" class="text-decoration">Home</a>
          </li>
          <li class="breadcrumb-item active" aria-current="page">
            <ol class="breadcrumb">
              <li class="breadcrumb-item">Data</li>
              <li class="breadcrumb-item active" aria-current="page">
                Add New Vehicle
              </li>
            </ol>
          </li>
        </ol>
      </nav>
    </div>
  </div>
  <div class="container my-3">
    <h5 class="orangeFont" style="text-align: start">
      APPROVE/REJECT UPLOADED PART PRICING
    </h5>
  </div>

  <div class="" style="overflow-x: Scroll">
    <table class="table table-hover">
      <thead class="bg-skyBlue btm-border">
        <tr>
          <th><input type="checkBox" /></th>
          <th scope="col">s.No</th>
          <th scope="col">Make</th>
          <th scope="col">Model</th>
          <th scope="col">Year</th>
          <th scope="col">Body Type</th>
          <th scope="col">Variant</th>
          <th scope="col">Part Std Name</th>
          <th scope="col">Oem Number</th>
          <th scope="col">Current Part Price</th>
          <th scope="col">Avg.Change Price</th>
          <th scope="col">Change Count</th>
          <th scope="col">Time Span</th>
          <th></th>
        </tr>
      </thead>
      <tbody>
        <TableRow slno="1" />
        <TableRow slno="2" />
        <TableRow slno="3" />
        <TableRow slno="4" />
        <TableRow slno="5" />
        <TableRow slno="6" />
        <TableRow slno="7" />
        <TableRow slno="8" />
        <TableRow slno="9" />
      </tbody>
    </table>
  </div>
  <div class="container d-felx" style="position: relative">
    <div class="pt-3">
      <nav aria-label="Page navigation example">
        <ul class="pagination justify-content-start">
          <li class="page-item disabled">
            <a class="page-link" href="#" tabindex="-1">Previous</a>
          </li>
          <li class="page-item"><a class="page-link" href="#">1</a></li>
          <li class="page-item"><a class="page-link" href="#">2</a></li>
          <li class="page-item"><a class="page-link" href="#">3</a></li>
          <li class="page-item">
            <a class="page-link" href="#">Next</a>
          </li>
          <li class="page-item">
            <a class="page-link" href="#">Last</a>
          </li>
        </ul>
      </nav>
    </div>
    <div
      class="container mt-2"
      style="text-align: end; position: absolute; top: 0"
    >
      <button
        type="button"
        class="btn btn-outline-primary m-2 px-5"
        style="border-color: #194a82; color: #194a82"
      >
        Reject
      </button>
      <button type="button" class="btn bg-theme-pr px-5">Approve</button>
    </div>
  </div>
</template>

<script>
import NavBar from "./NavBar.vue";
import TableRow from "./ReUsableComponents/TableRow.vue";
export default {
  name: "UploadPricing",
  components: {
    NavBar,
    TableRow,
  },
};
</script>

<style scoped>
.bg-skyBlue {
  background-color: #f5f9fd;
}
.bg-theme-pr {
  background-color: #194a82 !important;
  color: white !important;
}
.color-theme-pr {
  color: #194a82;
}
.orangeFont {
  color: #ffa200;
}
.select {
  padding: 6px;

  border-radius: 5px;
  border-color: #194a82;
  /* box-shadow: 0px 0px 5px 2px #b6c5d6; */
}
.text-decoration {
  text-decoration: none;
  color: #194a82;
  font-weight: 600;
}
.btm-border {
  border-bottom: 1px solid #b6c5d6 !important;
}
</style>