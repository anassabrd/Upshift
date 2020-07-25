<template>
  <div class="nav-bar bg-grey w-100">
    <b-navbar toggleable="lg" class="py-4">
      <b-navbar-brand class="w-20">Upshift</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav class="d-md-none d-lg-flex justify-content-between w-20">
        <b-navbar-nav class>
          <div class="d-flex align-items-center mr-3">
            <svg
              width="1.5em"
              height="1.5em"
              viewBox="0 0 16 16"
              class="bi bi-circle-fill bcf-1"
              fill="currentColor"
              xmlns="http://www.w3.org/2000/svg"
            >
              <circle cx="8" cy="8" r="8" />
            </svg>
            <b-nav-item class="d-inline" href="#">Personal</b-nav-item>
          </div>
          <div class="d-flex align-items-center ml-3">
            <svg
              width="1.5em"
              height="1.5em"
              viewBox="0 0 16 16"
              class="bi bi-circle-fill bcf-2"
              fill="currentColor"
              xmlns="http://www.w3.org/2000/svg"
            >
              <circle cx="8" cy="8" r="8" />
            </svg>
            <b-nav-item class="d-inline" href="#">Business</b-nav-item>
          </div>
        </b-navbar-nav>

        <b-navbar-nav class="w-50">
          <b-nav-item class="w-20" href="#">About</b-nav-item>
          <b-nav-item class="w-20" href="#">Pricing</b-nav-item>
          <b-nav-item class="w-20" href="#">FAQ</b-nav-item>
          <b-nav-item class="w-20" href="#">Contact Us</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="d-flex align-items-center w-20">
          <b-nav-item class="w-50" href="#">Login</b-nav-item>
          <b-nav-item class="w-50 btn btn-card py-3" href="#">Join now</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {};
</script>

<style>
.btn-card {
  border-radius: 30px !important;
  background-color: #e2e1e6 !important;
  color: white !important;
}

.nav-bar {
  position: fixed;
  z-index: 1000;
}

.w-20 {
  width: 20%;
}

.bcf-1 {
  fill: #72738e;
  display: inline;
}

.bcf-2 {
  fill: #e2e1e6;
  display: inline;
}

.nav-link {
  display: inline !important;
}
</style>