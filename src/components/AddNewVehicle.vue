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
    <h5 class="orangeFont" style="text-align: start">ADD NEW VEHICLE</h5>
  </div>

  <div class="container" style="text-align: start; width: 70%">
    <div class="row" style="justify-content: space-around">
      <div class="form-group col-md-5 d-flex align-items-center">
        <div class="col-8">
          <label for="inputCity" style="margin-left: 12px !important">
            <span
              class="h6 small pt-1 pl-2 pr-2"
              style="background-color: white"
              >Select Make</span
            >
          </label>
          <select
            id="inputCity"
            class="form-control"
            style="margin-top: -12px !important"
          >
            <option>Honda_ZX</option>
            <option>...</option>
          </select>
        </div>
        <div class="col-4" style="padding-left: 10px; margin-top: 10px">
          <button
            type="button"
            class="btn bg-theme-pr px-5"
            style="width: 100%"
          >
            Add
          </button>
        </div>
      </div>
      <div class="form-group col-md-3">
        <label for="inputState" style="margin-left: 12px !important">
          <span class="h6 small pt-1 pl-2 pr-2" style="background-color: white"
            >Select Variant</span
          >
        </label>
        <select
          id="inputState"
          class="form-control"
          style="margin-top: -12px !important"
        >
          <option selected>Choose...</option>
          <option>...</option>
        </select>
      </div>
    </div>
    <div class="row mt-3" style="justify-content: space-around">
      <div class="form-group col-md-5 d-flex align-items-center">
        <div class="col-8">
          <label for="inputCity" style="margin-left: 12px !important">
            <span
              class="h6 small pt-1 pl-2 pr-2"
              style="background-color: white"
              >Select Model</span
            >
          </label>
          <input
            type="text"
            style="margin-top: -12px !important"
            class="form-control"
            id="inputCity"
          />
        </div>
        <div class="col-4" style="padding-left: 10px; margin-top: 10px">
          <button
            type="button"
            class="btn bg-theme-pr px-5"
            style="width: 100%"
          >
            Add
          </button>
        </div>
      </div>
      <div class="form-group col-md-3">
        <label for="inputState" style="margin-left: 12px !important">
          <span class="h6 small pt-1 pl-2 pr-2" style="background-color: white"
            >Select Variant</span
          >
        </label>
        <select
          id="inputState"
          class="form-control"
          style="margin-top: -12px !important"
        >
          <option selected>Choose...</option>
          <option>...</option>
        </select>
      </div>
    </div>
    <div class="row mt-3" style="justify-content: space-around">
      <div class="form-group col-md-5">
        <label for="inputCity" style="margin-left: 12px !important">
          <span class="h6 small pt-1 pl-2 pr-2" style="background-color: white"
            >Select Year</span
          >
        </label>
        <input
          type="text"
          class="form-control"
          id="inputCity"
          style="margin-top: -12px !important"
        />
      </div>
      <div class="form-group col-md-3">
        <label for="inputState" style="margin-left: 12px !important">
          <span class="h6 small pt-1 pl-2 pr-2" style="background-color: white"
            >Select Variant</span
          >
        </label>
        <select
          id="inputState"
          class="form-control"
          style="margin-top: -12px !important"
        >
          <option selected>Choose...</option>
          <option>...</option>
        </select>
      </div>
    </div>
    <div class="row mt-3" style="justify-content: space-around">
      <div class="form-group col-md-5">
        <div
          class="d-flex"
          style="justify-content: space-between; align-items: center"
        >
          <div class="col-6">
            <label for="inputCity" style="margin-left: 12px !important">
              <span
                class="h6 small pt-1 pl-2 pr-2"
                style="background-color: white"
                >Year Range From</span
              >
            </label>
            <input
              type="text"
              class="form-control"
              id="inputCity"
              style="margin-top: -12px !important"
            />
          </div>
          <div class="col-1" style="text-align: center">To</div>
          <div class="col-5">
            <label for="inputCity" style="margin-left: 12px !important">
              <span
                class="h6 small pt-1 pl-2 pr-2"
                style="background-color: white"
                >Year Range To</span
              >
            </label>
            <input
              type="text"
              class="form-control"
              style="margin-top: -12px !important"
            />
          </div>
        </div>
      </div>

      <div class="form-group col-md-3">
        <label for="inputState" style="margin-left: 12px !important">
          <span class="h6 small pt-1 pl-2 pr-2" style="background-color: white"
            >Select Variant</span
          >
        </label>
        <select
          id="inputState"
          class="form-control"
          style="margin-top: -12px !important"
        >
          <option selected>Choose...</option>
          <option>...</option>
        </select>
      </div>
    </div>
    <div class="container mt-5" style="text-align: end; width: 85%">
      <button
        type="button"
        class="btn btn-outline-primary m-2 px-5"
        style="border-color: #194a82; color: #194a82"
      >
        Cancel
      </button>
      <button type="button" class="btn bg-theme-pr px-5">Save</button>
    </div>
  </div>
</template>

<script>
import NavBar from "./NavBar.vue";
export default {
  name: "AddNewVehicle",
  components: { NavBar },
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
  border-bottom: 1px solid #b6c5d6;
}
</style>