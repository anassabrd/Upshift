<template>
  <div class="container-fluid bg-grey">
    <div class="row align-items-center">
      <div class="col-3 mx-auto text-left">
        <div-title :num="'05'" :title="'the car'"></div-title>

        <h2 class="dark-blue mt-4">Always Drive an Identical Prius</h2>

        <div-body :part1="part1" :part2="part2"></div-body>
      </div>
      <div class="col-5 overlay-column">
        <div class="row">
          <div class="col-11 text-left pb-3">
            <img src="../../assets/images/3044520.jpg" class="w-100" alt />
          </div>
          <div class="col-5 text-left pt-3 pr-3">
            <img src="../../assets/images/3044536.jpg" class="w-100" alt />
          </div>
          <div class="col-7 text-left pl-3 pt-3">
            <img src="../../assets/images/14245.jpg" class="w-100" alt />
          </div>
        </div>
      </div>
    </div>

    <div class="row align-items-center mt-5 py-5">
      <div class="col-5 mx-auto">
        <h2 class="dark-blue">Join instantly with SO down and get your car right now.</h2>
      </div>
      <div class="col-5">
        <a href="#" class="btn btn-card mb-4 w-50 py-3">Get started</a>
      </div>
    </div>

    <hr class="my-0 w-75" />
  </div>
</template>

<script>
import divTitle from "@/components/divTitle";
import divBody from "@/components/divBody";

export default {
  components: {
    divTitle,
    divBody,
  },
  data() {
    return {
      part1:
        "All our cars are the same so they feel familiar. No branding so you don’t stick out.",
      part2:
        " Fits 5 comfortably — or a surfboard, bicycle, or skiis. 54 MPG hybrid gets you to Tahoe and back on a single tank. Phone mount, charging cables, and FasTrak included. Bluetooth and safety technology like adaptive cruise control. We use all natural deodorizers and cleaning supplies.",
    };
  },
};
</script>

<style>
.btn-card {
  border-radius: 30px !important;
  background-color: #72738e !important;
  color: #f6f5f8 !important;
}
.dark-blue {
  color: #333456;
}

.bg-grey {
  background-color: #f6f5f8;
}

.divider {
  background-color: #e4e4eb !important;
}

.overlay-column {
  margin-top: -8rem;
}

.w-30 {
  width: 30%;
}
</style>