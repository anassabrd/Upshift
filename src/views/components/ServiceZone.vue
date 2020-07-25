<template>
  <div class="container-fluid bg-grey">
    <div class="row px-5">
      <div class="col-5 overlay-image">
        <img src="../../assets/images/2792873.jpg" class="w-100" alt />
      </div>
      <div class="col-7 underlay-container">
        <div class="service-zone">
          <div-title :num="'03'" :title="'service-zone'" class="text-light-grey"></div-title>

          <h2 class="text-light mt-4">We’ve got SF covered</h2>

          <div-body :part1="part31" class="text-white-50"></div-body>

          <div-check :checkTitle="checkTitle1" :checkBody="checkBody1"></div-check>

          <div-check :checkTitle="checkTitle2" :checkBody="checkBody2"></div-check>

          <hr class="bg-grey my-5" />

          <div-footer :part3="part32" :part4="part33" class="text-light-grey"></div-footer>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import divTitle from "@/components/divTitle";
import divFooter from "@/components/divFooter";
import divBody from "@/components/divBody";
import divCheck from "@/components/divCheck";

export default {
  components: {
    divTitle,
    divFooter,
    divBody,
    divCheck,
  },
  data() {
    return {
      part31: "We provide two delivery options for any trip:",
      part32: "Outside of SF?",
      part33: "Tell us where to expand ",
      checkTitle1: "Concierge service (8am - 8pm daily)",
      checkBody1:
        "We deliver or pick up at your doorstep. Always have a parking spot right out front, just for you.",
      checkTitle2: "Self service (24/7)",
      checkBody2:
        "We deliver within 3 blocks and unlock it whenever you are ready. Park anywhere legal in our zone, lock up, and walk away to return. More flexibility on timing, especially for starting early or ending late.",
    };
  },
};
</script>

<style>
.bg-grey {
  background-color: #f6f5f8;
}

.text-light-grey {
  color: #f8f8fa;
}

.text-grey {
  color: #72738e;
}

.underlay-container {
  margin: 7rem -7rem -7rem;
  background-color: #333456;
  z-index: 10;
}

.overlay-image {
  z-index: 20;
  margin-left: 4rem;
}

.service-zone {
  width: 50%;
  text-align: left;
  margin: 5rem auto;
}
</style>