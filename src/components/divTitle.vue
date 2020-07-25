<template>
  <div class="title-box text-uppercase">
        <div class="title-num mr-4">{{num}}</div>
        <div class="divider"></div>
        <div class="title ml-4">{{title}}</div>
    </div>
</template>

<script>
export default {
  props: ["num", "title"]
};
</script>

<style scoped>
.title-box {
  display: flex;
  flex-direction: row;
  align-items: center;
  font-size: 12px !important;
  font-weight: 800 !important;
  line-height: 1em !important;
  letter-spacing: 2px !important;
  color: #72738e;
}

.left-border {
  border-left-color: #72738e !important;
  border-left-style: solid;
  border-left-width: 2px;
}

.title-num {
  flex-grow: 0;
}

.title {
  flex-grow: 2;
}

.divider {
  width: 70px;
  height: 2px;
  background-color: #f6f5f8;
}
</style>