<template>
  <header :class="`site-header-one stricky site-header-one__fixed-top ${sticky ? 'stricked-menu stricky-fixed' : ''}`">
    <div class="container-fluid nopadding">
      <div class="site-header-one__logo">
        <a href="/">
          <img src="/assets/images/bb_logo_v6.png" width="170" alt="">
        </a>
        <span @click="mobileToggle = !mobileToggle" class="side-menu__toggler"><i class="fa fa-bars"></i></span><!-- /.side-menu__toggler -->
      </div><!-- /.site-header-one__logo -->
      <div class="main-nav__main-navigation">
        <ul class="main-nav__navigation-box one-page-scroll-menu">
          <li class="scrollToLink">
            <a href="#home">Home</a>
          </li>
          <li class="scrollToLink"><a href="#features">Features</a></li>
          <li class="scrollToLink"><a href="#pricing">Pricing</a></li>
          <li class="scrollToLink"><a href="#team">Team</a></li>
          <!-- <li class="scrollToLink"><a href="#screens">Screens</a></li> -->
<!--           <li class="dropdown scrollToLink">
            <a href="#blog">News</a>
            <ul>
              <li><nuxt-link to="/blog">News</nuxt-link></li>
              <li><nuxt-link to="/blog-details">News Details</nuxt-link></li>
            </ul>
          </li> -->
        </ul><!-- /.main-nav__navigation-box -->
      </div><!-- /.main-nav__main-navigation -->
      <div class="main-nav__right">
        <a href="https://app.bbooster.net" class="thm-btn main-nav__btn"><span>Register Now</span></a>
      </div><!-- /.main-nav__right -->
    </div><!-- /.container-fluid -->

    <nav class="mobile-nav__container">
      <!-- content is loading via js -->

      <ul :style="`display: ${mobileToggle ? 'block' : 'none'}`" class="main-nav__navigation-box one-page-scroll-menu">
        <li class="scrollToLink">
          <a href="#home">Home</a>
        </li>
        <li class="scrollToLink"><a href="#features">Features</a></li>
        <li class="scrollToLink"><a href="#pricing">Pricing</a></li>
        <li class="scrollToLink"><a href="#team">Team</a></li>
        <li class="scrollToLink"><a href="#screens">Screens</a></li>
        <li class="dropdown scrollToLink">
          <a href="#blog">News</a>
          <ul>
            <li><nuxt-link to="/blog">News</nuxt-link></li>
            <li><nuxt-link to="/blog-details">News Details</nuxt-link></li>
          </ul>
        </li>
      </ul><!-- /.main-nav__navigation-box -->
    </nav>


  </header>
</template>

<script>
    export default {
      name: "Nav",
      data(){
        return {
          sticky: false,
          mobileToggle: false
        }
      },
      mounted() {
        window.addEventListener('scroll', this.handleScroll);
      },
      methods: {

        handleScroll() {
          if (window.scrollY > 70) {
            this.sticky = true
          } else if (window.scrollY < 70) {
            this.sticky = false
          }
        },
      }
    }
</script>

<style scoped>
.nopadding {
  padding-top: 5px!important;
  padding-bottom: 5px!important;
}
</style>
