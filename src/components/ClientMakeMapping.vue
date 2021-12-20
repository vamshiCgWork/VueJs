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
            CG-Client data Mapping
          </li>
        </ol>
      </nav>
    </div>
  </div>
  <div class="container my-3">
    <h5 class="orangeFont" style="text-align: start">CG-CLIENT MAKE MAPPING</h5>
  </div>

  <div class="container-fluid bg-skyBlue btm-border mt-5">
    <div class="container" style="text-align: start">
      <div class="row py-2">
        <div class="col">Client Make</div>
        <div class="col">CG-Standard-Make</div>
      </div>
    </div>
  </div>
  <div class="container-fluid btm-border">
    <div class="container" style="text-align: start">
      <div class="row py-2">
        <div class="col pt-1">BenZ</div>
        <div class="col">
          <select class="select">
            <option selected>Mercedes Benz</option>
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
        <div class="col pt-1">Chevy</div>
        <div class="col">
          <select class="select">
            <option selected>Cheverlot</option>
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
        <div class="col">
          <select class="select">
            <option>Choose...</option>
            <option selected>MG</option>
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
</template>

<script>
import NavBar from "./NavBar.vue";
export default {
  name: "ClientMakeMapping",
  components: {
    NavBar,
  },
};
</script>

<style scoped>
.bg-skyBlue {
  background-color: #f5f9fd;
}
.bg-theme-pr {
  background-color: #194a82;
  color: white;
}
.color-theme-pr {
  color: #194a82;
}
.orangeFont {
  color: #ffa200;
}
.select {
  padding: 6px;
  width: 35%;
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