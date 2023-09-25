<script>
export default {
name:"ProductItem",
props: ["image", "title", "price", "type"]
}
</script>

<template>
    <div class="col pt-5">
        <div class="card h-50 comics">
            <img :src="image" alt="" class="card-img-top h-100">
            <div class="card-bottom">
                <h5>{{ title }}</h5>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/Partials/variables' as *;
.comics {
   background-color: unset;
   border: none;
   color: $dc_white;
}

</style>