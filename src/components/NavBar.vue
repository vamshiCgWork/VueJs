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
</style>