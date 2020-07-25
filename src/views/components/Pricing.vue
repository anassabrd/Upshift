<template>
  <div class="container-fluid bg-white">
    <div class="pricing">
      <div-title :num="'04'" :title="'pricing'" class="text-light-grey w-10 mx-auto my-5"></div-title>

      <h1 class="pb-4">Monthly plans for less than a packing space.</h1>
      <p class="pb-4">
        Plans include concierge delivery and pickup, cleaning and refueling service, full coverage
        <br />and maintenance - everything but gas and tolls. Join instantly with SO down and get your car right now.
      </p>
      <div class="container mb-3">
        <div class="row align-items-end">
          <pricing-card
            :type="'FlexPass'"
            :recommended="false"
            :daysInMonth="2"
            :price="159"
            :description="descriptionFlexPass"
          ></pricing-card>
          <pricing-card
            :type="'Getaway'"
            :recommended="true"
            :daysInMonth="4"
            :price="219"
            :description="descriptionGetaway"
          ></pricing-card>
          <pricing-card
            :type="'Freedom'"
            :recommended="false"
            :daysInMonth="8"
            :price="389"
            :description="descriptionFreedom"
          ></pricing-card>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import pricingCard from "@/components/pricingCard";
import divTitle from "@/components/divTitle";

export default {
  components: {
    pricingCard,
    divTitle,
  },
  data() {
    return {
      descriptionFlexPass:
        "Not sure how much you drive? Get a magic button anytime need a car.",
      descriptionGetaway:
        "Get away up to once a week. your card is delivered and disappears like magic.",
      descriptionFreedom:
        "Get a car up to twice a week, " +
        "it's freedom whenever you want it (and no additional fees when you don't).",
    };
  },
};
</script>

<style>
.pricing {
  padding-top: 10rem;
  padding-bottom: 10rem;
}

.w-10 {
  width: 10%;
}
</style>