<template>
  <nav
    class="navbar navbar-expand-lg navbar-dark"
    style="background-color: #194a82"
  >
    <div class="container-fluid">
      <button class="btn"><span class="navbar-toggler-icon"></span></button>
      <div class="collapse navbar-collapse" id="navbarScroll">
        <ul
          class="navbar-nav me-auto my-2 my-lg-0 navbar-nav-scroll"
          style="--bs-scroll-height: 100px"
        >
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#"
              >CLAIM GENIUS</a
            >
          </li>
          <div class="nav-item" style="color: #9fb0cb; font-size: 25px">|</div>
          <li class="nav-item">
            <a class="nav-link active" href="#">PADAS MANAGEMENT TOOL</a>
          </li>
        </ul>
        <img src="../assets/avatar.png" alt="avatar" class="avatar" />
      </div>
    </div>
  </nav>
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
      <!-- <div class="card w-50">
      <div class="card-header">Featured</div>
      <div class="card-body">
        <h5 class="card-title">Special title treatment</h5>
        <p class="card-text">
          With supporting text below as a natural lead-in to additional content.
        </p>
        <a href="#" class="btn btn-primary">Go somewhere</a>
      </div>
    </div>
    <div class="card" style="width: 18rem">
      <div class="card-body">
        <h5 class="card-title">Card title</h5>
        <h6 class="card-subtitle mb-2 text-muted">Card subtitle</h6>
        <p class="card-text">
          Some quick example text to build on the card title and make up the
          bulk of the card's content.
        </p>
        <a href="#" class="card-link">Card link</a>
        <a href="#" class="card-link">Another link</a>
      </div>
    </div> -->
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
export default {
  setup() {},
};
</script>


<style scoped>
.avatar {
  vertical-align: middle;
  width: 50px;
  height: 50px;
  border-radius: 50%;
}
.fontAwe {
  font-family: Arial, FontAwesome;
}
.header-space {
  padding: 1rem 1rem;
}
</style>