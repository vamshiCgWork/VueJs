<template>
  <NavBar />
  <div class="container d-flex flex-column align-items-center fontAwe">
    <section
      class="d-flex my-5 align-items-start"
      style="flex-direction: column; width: 40%"
    >
      <div for="search" class="text-muted small mb-2">
        Select the Client for which you would like to review / moderate data
      </div>
      <div style="width: 100%">
        <form class="d-flex" style="width: 100%; margin: auto">
          <input
            class="form-control me-2"
            type="search"
            placeholder="&#xF002;"
            aria-label="Search"
          />
          <div class="dropdown">
            <button
              class="btn btn-secondary dropdown-toggle"
              type="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            ></button>
          </div>
        </form>
      </div>
    </section>
    <section style="width: 80%">
      <div class="row row-cols-1 row-cols-md-3 g-4">
        <div class="col">
          <div
            class="card"
            style="
              background-color: #1a4c81;
              color: white;
              border-radius: 8px;
              box-shadow: 0 8px 5px #ddd9da;
            "
          >
            <div
              class="header-space d-flex align-items-center"
              style="justify-content: space-between"
            >
              <div class="date" style="font-size: 12px">
                Start Date: 12/07/2021
              </div>
              <div
                class="notification"
                style="
                  width: 20px;
                  height: 20px;
                  border-radius: 20px;
                  background-color: #ffa200;
                "
              ></div>
            </div>
            <div class="card-body">
              <h1 class="card-title mb-4" style="color: #ffa200">12</h1>
              <h5 class="my-3" style="padding: 0 50px">
                Mapping of Make in progress
              </h5>
              <a
                class="btn btn-outline-secondary my-3"
                style="color: white; border-color: white; font-size: 12px"
                >Approve/Reject
                <span style="font-size: 15px; margin-left: 0.8rem"
                  >&#8594;</span
                >
              </a>
            </div>
          </div>
        </div>
        <div class="col">
          <div
            class="card"
            style="
              background-color: #419677;
              color: white;
              border-radius: 8px;
              box-shadow: 0 8px 5px #ddd9da;
            "
          >
            <div
              class="header-space d-flex align-items-center"
              style="justify-content: space-between"
            >
              <div class="date" style="font-size: 12px">
                Start Date: 12/07/2021
              </div>
              <div
                class="notification"
                style="
                  width: 20px;
                  height: 20px;
                  border-radius: 20px;
                  background-color: #ffa200;
                "
              ></div>
            </div>
            <div class="card-body">
              <h1 class="card-title mb-4">16</h1>
              <h5 class="my-3" style="padding: 0 50px">
                Mapping of Make in progress
              </h5>
              <a
                class="btn btn-outline-secondary my-3"
                style="color: white; border-color: white; font-size: 12px"
                >Approve/Reject
                <span style="font-size: 15px; margin-left: 0.8rem"
                  >&#8594;</span
                >
              </a>
            </div>
          </div>
        </div>

        <div class="col">
          <div
            class="card"
            style="
              background-color: #65468c;
              color: white;
              border-radius: 8px;
              box-shadow: 0 8px 5px #ddd9da;
            "
          >
            <div
              class="header-space d-flex align-items-center"
              style="justify-content: space-between"
            >
              <div class="date" style="font-size: 12px">
                Start Date: 12/07/2021
              </div>
              <div
                class="notification"
                style="
                  width: 20px;
                  height: 20px;
                  border-radius: 20px;
                  background-color: #ffa200;
                "
              ></div>
            </div>
            <div class="card-body">
              <h1 class="card-title mb-4" style="color: #ffa200">3</h1>
              <h5 class="my-3" style="padding: 0 50px">
                Mapping of Vehicle code is in progress
              </h5>
              <a
                class="btn btn-outline-secondary my-3"
                style="color: white; border-color: white; font-size: 12px"
                >Approve/Reject
                <span style="font-size: 15px; margin-left: 0.8rem"
                  >&#8594;</span
                >
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import NavBar from "./NavBar.vue";
export default {
  name: "DashBoard",
  components: {
    NavBar,
  },
  setup() {},
};
</script>


<style scoped>
.fontAwe {
  font-family: Arial, FontAwesome;
}
.header-space {
  padding: 1rem 1rem;
}
</style>