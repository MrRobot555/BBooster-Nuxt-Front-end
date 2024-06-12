<template>
  <div>
  <footer class="site-footer">
    <div class="site-footer__upper">
      <div class="container">
        <div class="row">
          <div class="col-lg-4">
            <div class="footer-widget footer-widget__about">
              <a href="/">
                <img src="/assets/images/bb_logo_v6.png" width="129" alt="">
              </a>
              <p>The key for your immediate 6 digit income
                <br>custom built for your business</p>
              <div class="f-legal-notice">This site is NOT endorsed by Facebook in any way.
FACEBOOK is a trademark of META</div>
            </div><!-- /.footer-widget -->
          </div><!-- /.col-lg-4 -->

          <div class="col-lg-5">
            <div class="footer-widget__links-wrap">
              <div class="footer-widget">
                <h3 class="footer-widget__title">Company</h3>
                <ul class="list-unstyled footer-widget__links-list">
                  <li><a href="#">About</a></li>
                  <li><a href="#">Our Team</a></li>
                  <li><a href="#">Contact</a></li>
                  <li><a href="#">Services</a></li>
                </ul><!-- /.list-unstyled footer-widget__links-list -->
              </div><!-- /.footer-widget -->
              <div class="footer-widget">
                <h3 class="footer-widget__title">Explore</h3>
                <ul class="list-unstyled footer-widget__links-list">
                  <!-- <li><a href="#">News</a></li> -->
                  <li><a href="#">Features</a></li>
                  <li><a href="#">Register</a></li>
                  <!-- <li><a href="#">Free Trial</a></li> -->
                </ul><!-- /.list-unstyled footer-widget__links-list -->
              </div><!-- /.footer-widget -->
              <div class="footer-widget">
                <h3 class="footer-widget__title">Legal</h3>
                <ul class="list-unstyled footer-widget__links-list">
                  <li><a href="https://app.bbooster.net/legal_docs/business_booster_privacy_policy.html">Privacy Policy</a></li>
                  <li><a href="https://app.bbooster.net/legal_docs/business_booster_terms_conditions.html">Terms of Use</a></li>
                  <li><a href="https://app.bbooster.net/legal_docs/company_details.html">Company details</a></li>
                </ul><!-- /.list-unstyled footer-widget__links-list -->
              </div><!-- /.footer-widget -->
            </div><!-- /.footer-widget__links-wrap -->
          </div><!-- /.col-lg-5 -->
<!--           <div
            class="col-lg-3 d-flex align-items-center justify-content-xl-end justify-content-lg-end justify-content-md-center justify-content-sm-center">
            <div class="footer-widget">
              <div class="footer-widget__social">
                <a href="#"><i class="fab fa-facebook-square"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-pinterest-p"></i></a>
              </div>
            </div>
          </div> -->
        </div><!-- /.row -->
      </div><!-- /.container -->
    </div><!-- /.site-footer__upper -->
    <div class="site-footer__bottom">
      <div class="container text-center">
        <p>© Copyright 2022 by Pompadur S.R.O. | E-mail: hello@bbooster.net | Phone: +436766747037</p>
      </div><!-- /.container -->
    </div><!-- /.site-footer__bottom -->
  </footer>

      <a @click="scrollTop" class="scroll-to-target scroll-to-top" :style="`display: ${scrollBtn ? 'inline' : 'none'}`" href="#"><i class="fa fa-angle-up"></i></a>


  </div>
</template>

<script>
    export default {
      name: "Footer",
      data(){
        return {
          scrollBtn: false
        }
      },
      mounted() {
        window.addEventListener('scroll', this.handleScroll);
      },

      methods: {

        handleScroll () {

          if (window.scrollY > 70) {
            this.scrollBtn = true
          }
          else if (window.scrollY < 70) {
            this.scrollBtn = false
          }
        },

        scrollTop () {
          window.scrollTo(0, 0);
        }


      }
    }
</script>

<style scoped>

</style>
