
<template>
  <section class="testimonials-one">
    <div class="container">
      <div class="row ">
        <div class="col-xl-6">
          <div class="testimonials-one__thumb-carousel-wrap">

            <div class="testimonials-one__icon">
              <div class="testimonials-one__icon-inner">
                <img src="/assets/images/shapes/testi-qoute-1-1.png" alt="">
              </div><!-- /.testimonials-one__icon-inner -->
            </div><!-- /.testimonials-one__icon -->
            <div class="testimonials-one__thumb-carousel">
              <div class="swiper-wrapper">
                <swiper :options="swiperOptions">
                  <swiper-slide>
                    <div class="swiper-slide">
                      <div class="testimonials-one__image">
                        <img src="/assets/images/resources/test1.jpg" alt="Awesome Image" />
                      </div><!-- /.testimonials-one__image -->
                    </div><!-- /.swiper-slide -->
                  </swiper-slide>
                  <swiper-slide>
                    <div class="swiper-slide">
                      <div class="testimonials-one__image">
                        <img src="/assets/images/resources/test2.jpg" alt="Awesome Image" />
                      </div><!-- /.testimonials-one__image -->
                    </div><!-- /.swiper-slide -->
                  </swiper-slide>
                  <swiper-slide>
                    <div class="swiper-slide">
                      <div class="testimonials-one__image">
                        <img src="/assets/images/resources/test3.jpg" alt="Awesome Image" />
                      </div><!-- /.testimonials-one__image -->
                    </div><!-- /.swiper-slide -->
                  </swiper-slide>
                </swiper>
              </div><!-- /.swiper-wrapper -->
            </div><!-- /.testimonials-one__thumb-carousel -->
          </div><!-- /.testimonials-one__thumb-carousel-wrap -->
        </div><!-- /.col-lg-6 -->
        <div class="col-xl-6 d-flex">
          <div class="my-auto">
            <div class="block-title text-left">
              <p>Our Testimonials</p>
              <h3>What Our Customers Are <br> Talking About</h3>
            </div><!-- /.block-title -->
            <div class="testimonials-one__carousel">
              <div class="swiper-wrapper">

                <swiper :options="swiperOptions">
                  <swiper-slide>
                    <div class="swiper-slide">
                      <div class="testimonials-one__single">
                        <p class="testimonials-one__text">I was a sells professional. I was constantly searching for new customers. Now I am just closing deals and started living a better life with whom I love. Thank you Business Booster! </p>
                        <!-- /.testimonials-one__text -->
                        <h3 class="testimonials-one__title">Joe Kolmer</h3>
                        <!-- /.testimonials-one__title -->
                      </div><!-- /.testimonials-one__single -->
                    </div><!-- /.swiper-slide -->
                  </swiper-slide>
                  <swiper-slide>
                    <div class="swiper-slide">
                      <div class="testimonials-one__single">
                        <p class="testimonials-one__text">I left my monthly subscription on auto renew, and enjoy the permanent flow of new clients. I spend on Business Booster, still I make more money than before. Please keep up the good work! </p>
                        <!-- /.testimonials-one__text -->
                        <h3 class="testimonials-one__title">Darrin Martos</h3>
                        <!-- /.testimonials-one__title -->
                      </div><!-- /.testimonials-one__single -->
                    </div><!-- /.swiper-slide -->
                  </swiper-slide>
                  <swiper-slide>
                    <div class="swiper-slide">
                      <div class="testimonials-one__single">
                        <p class="testimonials-one__text">I love this. I was so tired telling the same story about my service over and over again. It is done by Business Booster and I feel so relieved. Thank you!</p>
                        <!-- /.testimonials-one__text -->
                        <h3 class="testimonials-one__title">Tammy Daniely</h3>
                        <!-- /.testimonials-one__title -->
                      </div><!-- /.testimonials-one__single -->
                    </div><!-- /.swiper-slide -->
                  </swiper-slide>
                </swiper>
              </div><!-- /.swiper-wrapper -->

              <div class="testimonials-one__pagination-wrap">
                <div class="swiper-pagination"></div>
              </div><!-- /.testimonials-one__pagination-wrap -->
            </div><!-- /.testimonials-one__carousel -->
          </div><!-- /.my-auto -->
        </div><!-- /.col-lg-6 -->
      </div><!-- /.row -->
    </div><!-- /.container -->
  </section>
</template>

<script>
  import { Swiper, SwiperSlide, directive } from 'vue-awesome-swiper'
  import 'swiper/css/swiper.css'

  export default {
    name: "Testimonial",
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
            delay: 8000,
            disableOnInteraction: false
          },
          pagination: {
            el: '.swiper-pagination',
            type: 'bullets',
            clickable: true
          },
        }
      }
    },
  }
</script>

<style scoped>

</style>
