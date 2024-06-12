<template>
  <section class="brand-one">
    <div class="container">
      <div class="brand-one__carousel">
        <swiper :options="swiperOptions">
          <swiper-slide>
        <div class="item">
          <img src="/assets/images/resources/logo_limbic.png" alt="">
        </div><!-- /.item -->
          </swiper-slide>
          <swiper-slide>
        <div class="item">
          <img src="/assets/images/resources/logo_mwr.png" alt="">
        </div><!-- /.item -->
          </swiper-slide>
        </swiper>
      </div><!-- /.brand-one__carousel owl-carousel thm__owl-carousel owl-theme -->
    </div><!-- /.container -->
  </section>
</template>


<script>
  import { Swiper, SwiperSlide, directive } from 'vue-awesome-swiper';
  import 'swiper/css/swiper.css';

  export default {
    name: "Brands",
    components: {
      Swiper,
      SwiperSlide
    },
    directives: {
      swiper: directive
    },
    data() {
      return {
        swiperOptions: {
          slidesPerView : 1,
          loop: true,
          speed: 1000,
          spaceBetween : 30,
          autoplay: {
            delay: 3000,
            disableOnInteraction: false
          },
          // Responsive breakpoints
          breakpoints: {
            1024:{
              slidesPerView : 1
            },
            768:{
              slidesPerView : 1
            },
            640:{
              slidesPerView : 1
            },
            320:{
              slidesPerView : 1
            }
          }
        }
      }
    },
  }
</script>

<style scoped>

</style>

<style>
 .swiper-slide {
   display: flex;
   justify-content: center;
 }
</style>