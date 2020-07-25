<template>
  <div>
      <div class="row">
          <div class="col-2">
              <svg width="2em" height="2em" viewBox="0 0 16 16" class="bi bi-check fill-grey" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd" d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.236.236 0 0 1 .02-.022z"/>
              </svg>
          </div>
          <div class="col-10">
              <p class="text-light">{{checkTitle}}</p>
              <p class="text-white-50 checkBody">{{checkBody}}</p>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    props: ["checkTitle", "checkBody"]
}</script>

<style>

.fill-grey {
  fill: #72738e;
}

.text-light-grey {
  color: #f8f8fa;
}

.checkBody{
    font-weight: 300 !important;
    font-size: 17px !important;
    line-height: 1.5rem !important;
}

</style>