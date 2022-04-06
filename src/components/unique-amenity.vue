<template>
<section class="amenity">
    <img :src="amenity.imgUrl" alt="">
    <h4 class="amenity-title">{{ amenity.title }}</h4>
    <p class="amenity-txt">{{ amenity.txt }}</p>
</section>
</template>

<script>


export default {
    props:{
        amenity: Object
    }
}
</script>

<style>

</style>