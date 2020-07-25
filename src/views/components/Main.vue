<template>
  <div class="container-fluid bg-grey">
    <div class="row">
      <div class="col-md-6">
        <div class="p-5 main-part d-flex justify-content-center flex-column text-left">
          <h1 class="pb-4" style="font-size: 3.5rem;">
            Just drive.
            <br />We'll do the rest.
          </h1>
          <h6 style="font-weight: 100">All inclusive, usage-based car subscriptions</h6>
          <div class="d-flex pt-3">
            <b-form-input class="mr-sm-2 main-input col-8" placeholder="Phone number..."></b-form-input>
            <b-button
              size="sm"
              class="my-2 my-sm-0 col-4"
              style="border-radius: 30px;"
              type="submit"
            >Get started</b-button>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <!-- X logo -->
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.bg-grey {
  background-color: #f6f5f8;
}

.main-part {
  height: 90vh;
}
.main-input {
  background-color: transparent;
  border: none;
  border-bottom: 1px solid #e8e8e8;
  border-radius: 0;
}

input:focus {
  background-color: transparent;
  border: none;
}

.get-started-button {
  border-radius: 30px;
}
</style>