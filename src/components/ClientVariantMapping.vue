<template>
  <NavBar />
  <div class="container-fluid bg-skyBlue">
    <div class="container">
      <nav aria-label="breadcrumb">
        <ol class="breadcrumb">
          <li class="breadcrumb-item">
            <a href="#" class="text-decoration">Utilities</a>
          </li>
          <li class="breadcrumb-item active" aria-current="page">
            CG-Std_Client Variant Mapping
          </li>
        </ol>
      </nav>
    </div>
  </div>

  <div class="container my-3">
    <h5 class="orangeFont" style="text-align: start">
      CG-CLIENT VARIANT MAPPING
    </h5>
  </div>

  <div class="container-fluid bg-skyBlue btm-border mt-5">
    <div class="container" style="text-align: start">
      <div class="row py-2">
        <div class="col">Client Make</div>
        <div class="col">Client Model</div>
        <div class="col">Client Variant</div>
        <div class="col">CG-Standard-Make</div>
        <div class="col">CG-Standard-Model</div>
        <div class="col">CG-Standard-Variant</div>
      </div>
    </div>
  </div>
  <div class="container-fluid btm-border">
    <div class="container" style="text-align: start">
      <div class="row py-2">
        <div class="col pt-1">Chevy</div>
        <div class="col pt-1">UVA</div>
        <div class="col pt-1">Zx</div>
        <div class="col pt-1">Cheverlot</div>
        <div class="col pt-1">UVA</div>
        <div class="col">
          <select class="select">
            <option selected>Zx</option>
            <option>Choose...</option>
            <option>...</option>
          </select>
        </div>
      </div>
    </div>
  </div>
  <div class="container-fluid btm-border">
    <div class="container" style="text-align: start">
      <div class="row py-2">
        <div class="col pt-1">BenZ</div>
        <div class="col pt-1">UVA</div>
        <div class="col pt-1">Zt</div>
        <div class="col pt-1">Mercedes Benz</div>
        <div class="col pt-1">UVC</div>
        <div class="col">
          <select class="select">
            <option selected>Zt</option>
            <option>Choose...</option>
            <option>...</option>
          </select>
        </div>
      </div>
    </div>
  </div>
  <div class="container-fluid btm-border">
    <div class="container" style="text-align: start">
      <div class="row py-2">
        <div class="col pt-1">Morris Garages</div>
        <div class="col pt-1">UVA</div>
        <div class="col pt-1">Lt</div>
        <div class="col pt-1">MG</div>
        <div class="col pt-1">LT</div>
        <div class="col">
          <select class="select">
            <option>Choose...</option>
            <option selected>Lt</option>
            <option>...</option>
          </select>
        </div>
      </div>
    </div>
  </div>

  <div class="container mt-2" style="text-align: end">
    <button
      type="button"
      class="btn btn-outline-primary m-2 px-5"
      style="border-color: #194a82; color: #194a82"
    >
      Reject
    </button>
    <button type="button" class="btn bg-theme-pr px-5">Approve</button>
  </div>

  <div class="">
    <table class="table">
      <thead class="thead bg-skyBlue">
        <tr>
          <th scope="col">Client Make</th>
          <th scope="col">Client Model</th>
          <th scope="col">Client Variant</th>
          <th scope="col">CG-Standard-Make</th>
          <th scope="col">CG-Standard-Model</th>
          <th scope="col">CG-Standard-Variant</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Chevy</td>
          <td>UVA</td>
          <td>Zx</td>
          <td>Cheverlot</td>
          <td>UVA</td>
          <td>
            <select class="select">
              <option selected>Zx</option>
              <option>Choose...</option>
              <option>...</option>
            </select>
          </td>
        </tr>
        <tr>
          <td>BenZ</td>
          <td>UVA</td>
          <td>Zt</td>
          <td>Mercedes Benz</td>
          <td>UVC</td>
          <td>
            <select class="select">
              <option selected>Zt</option>
              <option>Choose...</option>
              <option>...</option>
            </select>
          </td>
        </tr>
        <tr>
          <td>Morris Garages</td>
          <td>UVA</td>
          <td>Lt</td>
          <td>MG</td>
          <td>LT</td>
          <td>
            <select class="select">
              <option selected>Lt</option>
              <option>Choose...</option>
              <option>...</option>
            </select>
          </td>
        </tr>
      </tbody>
    </table>
    <div class="container mt-2" style="text-align: end">
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
export default {
  name: "ClientVariantMapping",
  components: { NavBar },
};
</script>

<style>
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