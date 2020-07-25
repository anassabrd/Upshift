<template>
  <div>
    <Main />
    <About />
    <HowTo />
    <ServiceZone />
    <Pricing />
    <TheCar />
  </div>
</template>

<script>
import About from "./components/About";
import Main from "./components/Main";
import HowTo from "./components/HowTo";
import ServiceZone from "./components/ServiceZone";
import Pricing from "./components/Pricing";
import TheCar from "./components/TheCar";
export default {
  name: "Home",
  components: {
    About,
    Main,
    HowTo,
    ServiceZone,
    Pricing,
    TheCar,
  },
};
</script>
