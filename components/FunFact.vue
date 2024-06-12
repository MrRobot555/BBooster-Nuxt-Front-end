<template>
  <section class="funfact-one" v-observe-visibility="onVisibilityChange">
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-md-6">
          <div class="funfact-one__single">
            <h3 class="counter"> > <countTo :startVal='0' :endVal='startCounter ? 300 : 0' :duration='3000'></countTo></h3>
            <p>Negotiations Daily</p>
          </div><!-- /.funfact-one__single -->
        </div><!-- /.col-lg-3 col-md-6 -->
        <div class="col-lg-4 col-md-6">
          <div class="funfact-one__single">
            <h3 class="counter"> > <countTo :startVal='0' :endVal='startCounter ? 50 : 0' :duration='3000'></countTo> %</h3>
            <p>Closed Deals</p>
          </div><!-- /.funfact-one__single -->
        </div><!-- /.col-lg-3 col-md-6 -->
        <div class="col-lg-4 col-md-6">
          <div class="funfact-one__single">
            <h3 class="counter"><countTo :startVal='0' :endVal='startCounter ? 24 : 0' :duration='3000'></countTo>/7</h3>
            <p>Hours Working Time</p>
          </div><!-- /.funfact-one__single -->
        </div><!-- /.col-lg-3 col-md-6 -->
<!--         <div class="col-lg-3 col-md-6">
          <div class="funfact-one__single">
            <h3 class="counter"><countTo :startVal='0' :endVal='startCounter ? 266 : 0' :duration='3000'></countTo></h3>
            <p>Awards</p>
          </div>
        </div> -->
      </div><!-- /.row -->
    </div><!-- /.container -->
  </section>
</template>

<script>
  import countTo from 'vue-count-to';
  import { ObserveVisibility } from 'vue-observe-visibility'

  export default {
    name: "FunFact",
    components: { countTo },
    directives: {
      ObserveVisibility
    },
    data() {
      return{
        startCounter: false
      }
    },
    methods: {
      onVisibilityChange (isVisible) {
        if (isVisible){
          this.startCounter = true;
        }

      },
    },
  }
</script>


<style scoped>

</style>
