<template>
  <div class="col-md-4 p-4">
    <article class="card d-flex" v-bind:class="{ 'card-shadow' : recommended }">
      <div class="card-body p-5">
        <div class="pb-4">
          <span
            v-bind:class="{ 'd-none' : !recommended }"
            class="text-uppercase recommended pb-5"
          >Recommended</span>
          <h3 class="card-title">{{type}}</h3>
          <span class="days">Get {{daysInMonth}} days/month</span>
        </div>
        <h2 class="price">${{price}}</h2>
        <span class="month">/month</span>
        <hr />
        <div class="pt-2">
          <p class="card-text pb-3 grey">{{description}}</p>
          <a href="#" class="btn btn-card mb-4 w-100 py-3">Start with {{type}}</a>
          <br />
          <a href="#" style="color: #72738e">Vien plan details -></a>
        </div>
      </div>
    </article>
  </div>
</template>

<script>
export default {
  props: ["type", "recommended", "daysInMonth", "price", "description"],
};
</script>

<style scoped>
.btn-card {
  border-radius: 30px;
  background-color: #72738e;
  color: white;
}
.card-shadow {
  box-shadow: 0px 60px 100px #e4e4eb;
  border-top: #72738e 3px solid !important;
  border: none;
}

.recommended {
  font-size: 13px;
  font-weight: 700;
  letter-spacing: 0.6px;
  color: #72738e;
}

.card-title {
  letter-spacing: 1px;
}

.card-text {
  font-size: 14px !important;
  letter-spacing: 0.5px !important;
  font-weight: 300 !important;
}

.price {
  font-weight: 500 !important;
  display: inline;
  color: #72738e;
}

.days {
  font-weight: 100 !important;
  font-size: 14px !important;
  color: #72738e;
}

.month {
  font-weight: 100 !important;
  font-size: 15px !important;
  color: #72738e;
}
</style>