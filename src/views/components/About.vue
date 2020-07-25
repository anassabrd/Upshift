<template>
  <div class="container-fluid bg-white">
    <div class="row p-5">
      <div class="col-6 p-5">
        <div class="overlay-container">
          <div class="overlay-review w-70 p-5">
            <div class="p-3">
              <p
                class="left-border text-left px-3"
              >"Since becoming a monthly subscriber, I feel like I have my car back again. It's like I own a car without the worries or cost of keeping it around all the time."</p>
            </div>
            <div class="row align-items-center">
              <div class="col-3 text-right">
                <img src="../../assets/images/rmv.png" class="w-50" alt />
              </div>
              <div class="col-2 px-0">
                <span class="float-left text-uppercase">sam r.</span>
              </div>
              <div class="col-7">
                <span class="float-right">28 revies at Yelp</span>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-4 p-5 text-left my-auto">
        <div-title :num="'01'" :title="'about-us'"></div-title>

        <h2 class="dark-blue mt-4">Let's make cities better</h2>

        <div-body :part1="part1" :part2="part2"></div-body>

        <hr class="grey my-5" />

        <div-footer :part3="part3" :part4="part4"></div-footer>
      </div>
    </div>
  </div>
</template>

<script>
import divTitle from "@/components/divTitle";
import divBody from "@/components/divBody";
import divFooter from "@/components/divFooter";

export default {
  components: {
    divTitle,
    divBody,
    divFooter,
  },
  data() {
    return {
      part1:
        "Upshift is like having your own car at your doorstep, but only the days you want it. Monthly plans based on how much you drive that include parking, insurance, maintenance and more.",
      part2:
        "We believe in using business to drive positive change in the world and never settling for what worked in the past.",
      part3: "Interested in our values?",
      part4: "Learn more about the company",
    };
  },
};
</script>

<style>
.dark-blue {
  color: #333456;
}

.dark-grey {
  color: #4d5361;
}

.bg-light-grey {
  background-color: #f8f8fa;
}

.grey {
  color: #72738e;
}

h2 {
  font-size: 2.5rem !important;
  line-height: 1.3em !important;
  font-weight: 500 !important;
  letter-spacing: normal !important;
}

.w-70 {
  width: 70%;
}

p {
  line-height: 2rem !important;
  letter-spacing: 0.2px !important;
  font-size: 18px !important;
  font-weight: 400 !important;
}

.left-border {
  border-left-color: #72738e !important;
  border-left-style: solid;
  border-left-width: 2px;
}

.overlay-container {
  background-image: url("../../assets/images/3044526.jpg");
  background-repeat: no-repeat;
  height: 600px;
  background-size: contain;
}

.overlay-review {
  background-color: #333456;
  color: white;
  bottom: -40px;
  position: absolute;
  left: 100px;
}
</style>