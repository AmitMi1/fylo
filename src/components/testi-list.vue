<template>
  <section class="testimonial-list ml">
      <div class="testimonials-container flex center">
          <unique-testi :testi="t" v-for="t in testimonialList" :key="t"></unique-testi>
      </div>
  </section>
</template>

<script>
import uniqueTesti from "./unique-testi.vue"

export default {
    props:{
        testimonialList: Array
    },
    components:{
        uniqueTesti
    }
}
</script>

<style>

</style>