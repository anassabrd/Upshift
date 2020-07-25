<template>
  <div class="col-3 p-4">
        <img src="../assets/images/rmv_light.png" class="w-25" alt="">

        <h3 class="option-title">{{title}}</h3>

        <p class="option-desc">{{desc}}</p>

        <hr>
    </div>
</template>

<script>
export default {
props: ["title", "desc"]
}
</script>

<style scoped>
.option {
	position: relative;
}

.option::after {
    content: "";
    width: 50%;
	position: absolute;
	top: 5rem;
	right: 0;
	-webkit-transform: translateX(55%);
	-ms-transform: translateX(55%);
	transform: translateX(55%);
	width: 50%;
	height: 26px;
	background-image: url(data:image/svg+xml;charset=UTF-8;base64,PHN2ZyB3aWR0aD0iMTU0IiBoZWlnaHQ9IjI2IiB2aWV3Qm94PSIwIDAgMTU0IDI2IiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxwYXRoIGQ9Ik0yIDJjMzIuMjYgMTMuNzUgNTguNiAyMS4xIDc5IDIyLjA0IDIwLjQuOTUgNDYuNzQtMy45NSA3OS0xNC43IiBzdHJva2U9IiMxNTI2NDciIHN0cm9rZS13aWR0aD0iMiIgZmlsbD0ibm9uZSIgZmlsbC1ydWxlPSJldmVub2RkIiBvcGFjaXR5PSIuMiIgc3Ryb2tlLWRhc2hhcnJheT0iNSwxMCIgc3Ryb2tlLWxpbmVjYXA9InNxdWFyZSIvPjwvc3ZnPg==);
	background-repeat: no-repeat;
}

.option:nth-child(2n)::after {
	top: 0;
	-webkit-transform: translateX(50%) scaleY(-1);
	-ms-transform: translateX(50%) scaleY(-1);
	transform: translateX(50%) scaleY(-1);
}

.option-title{
    padding: 3rem 0rem 1rem;

}

.option-desc {
    color: #72738e;
    padding-bottom: 2rem;
}
</style>