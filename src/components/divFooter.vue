<template>
  <div>

    <div class="row align-items-center">
        <div class="col-2 px-0">
        <img src="../assets/images/rmv.png" class="w-70" alt="">
        </div>
        <div class="col-10">
        <span>{{part3}}</span> <br>
        <span>{{part4}}</span>
        </div>
    </div>
  </div>
        
</template>

<script>
export default {
    props: ["part3", "part4"]
}
</script>

<style scoped>

.w-70 {
  width: 70%;
}

</style>