<template>
  <div class="container-fluid bg-light-grey">
    <div class="row p-5">
      <div class="col-4 p-5 text-left my-auto">
        <div-title :num="'02'" :title="'how it works'"></div-title>

        <h2 class="dark-blue mt-4">Simple and handy rental process</h2>
      </div>
      <div class="col-4 p-5 text-left">
        <div-body :part1="part11"></div-body>

        <hr class="grey my-5" />

        <div-footer :part3="part13"></div-footer>
      </div>
      <div class="col-4 p-5 text-left">
        <div-body :part1="part21"></div-body>

        <hr class="grey my-5" />

        <div-footer :part3="part23"></div-footer>
      </div>
    </div>
    <div class="row p-5">
      <div-option :title="'Text us'" :desc="desc1" class="option"></div-option>

      <div-option :title="'We deliver'" :desc="desc2" class="option mt-5"></div-option>

      <div-option :title="'You drive'" :desc="desc3" class="option"></div-option>

      <div-option :title="'We pick It Up'" :desc="desc4" class="mt-5"></div-option>
    </div>
  </div>
</template>

<script>
import divTitle from "@/components/divTitle";
import divBody from "@/components/divBody";
import divFooter from "@/components/divFooter";
import divOption from "@/components/divOption";

export default {
  components: {
    divTitle,
    divBody,
    divOption,
    divFooter,
  },
  data() {
    return {
      part11:
        "Snow chains, surf board rack, key lock box, or dog car seat hammock available upon request.",
      part13: "Check the available accessories",
      part21:
        "Still got questions? We've probably covered them all in the Help Center.",
      part23: "Read our FAQ",
      desc1:
        "Text when you want your car. No app needed, just an online account. Real human operators.",
      desc2: "Your car will arrive at your door - clean and fully fueled",
      desc3:
        "Hop in and go with full coverage insurance, FasTrak, phone accessories, and unlimited mileage",
      desc4:
        "It's yours for a few hours or a few days. Return on your own time, anywhere in We'll gas and clean it.",
    };
  },
};
</script>

<style>
.bg-light-grey {
  background-color: #fdfdfd;
}
</style>