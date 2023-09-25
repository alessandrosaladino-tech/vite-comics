<script>
export default {
    name: "ProductItem",
    props: ["image", "title", "price", "type"]
}
</script>

<template>
    <a href="##">
        <div class="col pt-5">
            <div class="card h-50 comics">
                <img :src="image" alt="" class="card-img-top card_img_h">
                <div class="card-bottom">
                    <h6 class="text-uppercase pt-2 title_fs">{{ title }}</h6>
                    <p>{{ price }}</p>
                </div>
            </div>
        </div>
    </a>
</template>


<style lang="scss" scoped>
@use '../assets/scss/Partials/variables' as *;

.comics {
    background-color: unset;
    border: none;
    color: $dc_white;
    border-radius: none;
}

.col {
    height: 10%;

    & .title_fs {
       font-size: 15px;
    }

    & p {
        font-size: 13px;
    }
}

.card_img_h {
    height: 200px;
}

p {
    color: $dc_primary;
}

a{
    text-decoration: none;
}
</style>