<template>
  <section class="amenity-list ml">
      <div class="amenity-container flex wrap">
          <unique-amenity :amenity="a" v-for="a in amenities" :key="a"></unique-amenity>
      </div>
  </section>
</template>

<script>

import uniqueAmenity from "./unique-amenity.vue"

export default {
    props: {
        amenities: Array
    },
    components:{
        uniqueAmenity,
    }
}
</script>

<style>

</style>