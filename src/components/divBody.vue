<template>
  <div>
    <p class="grey mt-4 body">{{part1}}</p>
    <p class="grey my-4 body">{{part2}}</p>
  </div>
</template>

<script>
export default {
  props: ["part1", "part2"],
};
</script>

<style scoped>
.grey {
  color: #72738e;
}

.body {
  font-weight: 350 !important;
}
</style>