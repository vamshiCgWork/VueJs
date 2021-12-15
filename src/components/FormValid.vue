<template>
  <div class="container-fluid h-100">
    <div class="row h-100">
      <div
        class="
          col-7
          primary
          h-100
          d-flex
          justify-content-center
          align-items-center
        "
        style="background-color: #275b95"
      >
        <div class="container" style="height: 100%">
          <div
            class="row justify-content-center"
            style="height: 100%; position: relative"
          >
            <div
              class="col-12"
              style="position: absolute; top: 10%; width: 60%"
            >
              <div class="row" style="color: white">
                <div class="col">PDAS MANAGMENT TOOL</div>
                <div class="col">PDAS MANAGMENT TOOL</div>
              </div>
            </div>
            <div
              class="col-12 d-flex justify-content-center align-items-center"
              style="height: 100%"
            >
              <img alt="Vue logo" src="../assets/logo.png" width="100" />
            </div>
          </div>
        </div>
      </div>
      <div
        class="col-5 d-flex justify-content-center align-items-center"
        style="background-color: #194a82; text-align: start"
      >
        <div class="box">
          <legend>Login</legend>
          <form
            autocomplete="off"
            class="row g-3 needs-validation"
            @submit="submitForm"
            novalidate
          >
            <div class="col-12 form-group input-group-lg">
              <label
                for="validationCustom01"
                class="col-sm-2"
                style="margin-left: 12px !important"
              >
                <span class="h6 small pt-1 pl-2 pr-2 loginColor">Team ID</span>
              </label>
              <input
                type="text"
                id="validationCustom01"
                required
                v-model.trim="state.teamid"
                :class="{
                  'is-invalid': v$.teamid.$error,
                  'is-valid': state.teamid !== '' && !v$.teamid.$invalid,
                }"
                class="form-control"
                style="margin-top: -12px !important"
              />
              <div class="valid-feedback">Looks good!</div>
              <div class="invalid-feedback">Required!</div>
            </div>
            <div class="col-12 form-group input-group-lg">
              <label
                for="validationCustom02"
                class="col-sm-2"
                style="margin-left: 12px !important"
              >
                <span class="h6 small pt-1 pl-2 pr-2 loginColor"
                  >UserName</span
                ></label
              >
              <input
                type="text"
                class="form-control"
                id="validationCustom02"
                required
                v-model.trim="state.username"
                :class="{
                  'is-invalid': v$.username.$error,
                  'is-valid': state.username !== '' && !v$.username.$invalid,
                }"
                style="margin-top: -12px !important"
              />
              <div class="valid-feedback">Looks good!</div>
              <div class="invalid-feedback">Required!</div>
            </div>

            <div class="col-12 form-group input-group-lg mb-3">
              <label
                for="validationCustom03"
                class="col-sm-2"
                style="margin-left: 12px !important"
              >
                <span class="h6 small pt-1 pl-2 pr-2 loginColor">Password</span>
              </label>
              <input
                type="password"
                id="validationCustom03"
                required
                v-model.trim="state.password"
                :class="{
                  'is-invalid': v$.password.$error,
                  'is-valid': state.password !== '' && !v$.password.$invalid,
                }"
                class="form-control"
                style="margin-top: -12px !important"
              />
              <div class="valid-feedback">Looks good!</div>
              <div class="invalid-feedback">Required!</div>
            </div>
            <p style="color: #e3fefe">Forgot Password ?</p>
            <div
              class="
                mt-5
                d-grid
                gap-2
                d-md-flex
                justify-content-between
                align-items-center
              "
            >
              <a href="#" class="link-primary" style="color: #e3fefe"
                >Don't have an account ?</a
              >
              <button class="btn" type="button" style="color: #e3fefe">
                SIGN UP
              </button>
            </div>
            <div class="col-12 d-grid mt-3">
              <button
                class="btn"
                style="background-color: #e3fefe; color: #194a82"
                type="submit"
              >
                SIGN IN
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import useValidate from "@vuelidate/core";
import { required } from "@vuelidate/validators";
import { reactive, computed } from "vue";
export default {
  setup() {
    const state = reactive({
      teamid: "",
      username: "",
      password: "",
    });
    const rules = computed(() => {
      return {
        teamid: { required },
        username: { required },
        password: { required },
      };
    });

    const v$ = useValidate(rules, state);

    return { state, v$ };
  },
  methods: {
    submitForm(e) {
      e.preventDefault();
      this.v$.$validate();
      if (!this.v$.$error) {
        console.log("formValues", this.state);
      } else {
        console.log(
          "errors",
          this.v$.username.$error,
          this.v$.username.$invalid,
          this.state.username
        );
      }
    },
  },
};
</script>

<style scoped>
.box {
  padding-left: 10%;
  padding-right: 30%;
  color: #e3fefe;
  height: 100%;
}
legend {
  margin: 20% 0;
}
input {
  background-color: transparent;
}
input:focus {
  background-color: #194a82;
}
.loginColor {
  background-color: #194a82;
  padding: 5px;
}
.row > * {
  margin-top: 0;
}
</style>