<template>
  <section class="testimonial">
    <p class="txt">{{ testi.txt }}</p>
    <div class="flex user">
    <img :src="testi.userImg" alt="">
    <div>
    <p class="fullname">{{ testi.fullname }}</p>
    <p class="user-title">{{ testi.userTitle }}</p>
    </div>
    </div>
  </section>
</template>

<script>
export default {
    props: {
        testi: Object
    }
}
</script>

<style>

</style>