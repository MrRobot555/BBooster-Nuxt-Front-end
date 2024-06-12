<template>
  <section class="banner-one" id="home">

    <img src="/assets/images/shapes/banner-shape-1-1.png" class="banner-one__bg-shape-1" alt="">
    <div class="banner-one__bg" style="background-image: url(/assets/images/resources/banner-pic.jpg)">

    </div><!-- /.banner-one__bg -->
    <div class="container">
<!--       <a href="https://www.youtube.com/watch?v=Kl5B6MBAntI" class="mediabox banner-one__video video-popup"><i
        class="fa fa-play"></i></a> -->
      <div class="banner-one__moc">
        <img src="/assets/images/resources/phone_v2.png" class="wow fadeInUp"
             data-wow-duration="1500ms" alt="">
      </div>
      <div class="row">
        <div class="col-lg-7">
          <div class="banner-one__content">
<!--             <form class="banner-one__mc-form mc-form" data-url="MAILCHIMP__POPUP__FORM__URL">
              <input type="text" name="email" placeholder="Email address">
              <button type="submit" class="thm-btn banner-one__mc-btn"><span>Free
                                        Trial</span></button><!-- /.thm-btn banner-one__mc-btn -->
            <!-- </form>
            <div class="mc-form__response"></div> --> <!-- /.mc-form__response -->
            <h3>The key<br> for your 6 digit business <br> performance</h3>
            <p>Ensure uninterrupted supply of clients <br> By simply ordering them
              interested and ready to order from you.</p>
            <a href="#" class="thm-btn banner-one__btn"><span>Try Business Booster</span></a>
            <!-- /.thm-btn banner-one__btn -->
          </div><!-- /.banner-one__content -->
        </div><!-- /.col-lg-7 -->
      </div><!-- /.row -->
    </div><!-- /.container -->
  </section>
</template>

<script>

    export default {
      name: "Banner",
      mounted() {
        MediaBox('.mediabox', { rel: '0' });
      }

    }
</script>

<style scoped>

</style>
