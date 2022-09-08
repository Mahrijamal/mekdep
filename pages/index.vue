<template>
  <div class="landing">
    <section class="home" id="home">
      <div class="hooper_main">
        <div class="hooper">
          <hooper :settings="hooperSettings">
            <slide>
              <div class="slider1">
                <div class="content"></div>
              </div>
            </slide>

            <slide>
              <div class="slider1 slider2">
                <div class="content"></div>
              </div>
            </slide>

            <slide>
              <div class="slider1 slider3">
                <div class="content"></div>
              </div>
            </slide>

            <slide>
              <div class="slider1 slider4">
                <div class="content"></div>
              </div>
            </slide>

            <slide>
              <div class="slider1 slider5">
                <div class="content"></div>
              </div>
            </slide>

            <slide>
              <div class="slider1 slider6">
                <div class="content"></div>
              </div>
            </slide>

            <hooper-navigation slot="hooper-addons"></hooper-navigation>
            <hooper-pagination slot="hooper-addons"></hooper-pagination>
            <hooper-progress slot="hooper-addons"></hooper-progress>
          </hooper>
        </div>
      </div>
    </section>

    <div class="map">
      <div class="title">
        <p>Bütündünýä olimpiada ýeňijelerimiz</p>
      </div>
      <div class="maps">
        <Map />
      </div>
    </div>

    <div class="new">
      <div class="news">
        <New />
      </div>
    </div>

    <div class="adds">
      <div class="ads">
        <Ads />
      </div>
    </div>

    <div class="ice_cream">
 
      <div class="cards">
        <Card v-for="(e, i) in products_ice" :key="i" :info="e" />
      </div>
    </div>
  </div>
</template>

<script>
import {
  Hooper,
  Slide,
  Progress as HooperProgress,
  Pagination as HooperPagination,
  Navigation as HooperNavigation,
} from 'hooper'
import 'hooper/dist/hooper.css'
import Card from '@/components/card.vue'
import Map from '@/components/map.vue'
import New from '@/components/new.vue'
import Ads from '@/components/ads.vue'

export default {
  components: {
    Hooper,
    Slide,
    HooperProgress,
    HooperPagination,
    HooperNavigation,
    Card,
    Map,
    New,
    Ads,
  },
  data() {
    const mainProducts = {
      ice_cream: {
        title: 'Klasyň hepdelik meýilnamasy',
        products5: [
          {
            id: 'Tebigat',
            img: 'matem',
            text: 'Rus-dili',
            price: 'Geografiya',
            conut: 'Taryh',
            date: 'English',
          },
        ],
      },
    }
    return {
      mainProducts,

      hooperSettings: {
        itemsToShow: 4,
        centerMode: false,
        autoPlay: true,
        playSpeed: 5000,
        transition: 1100,
        hoverPause: false,
        infiniteScroll: true,
        wheelControl: false,
      },
    }
  },
  // created(){
  //   this.$store.dispatch('set_products', this.mainProducts.ice_cream)
  // },
  computed: {
    products_ice() {
      return this.$store.getters.products12
    },
  },
}
</script>

<style>
.landing {
  width: 1440px;
  margin: 0 auto;
}
.hooper {
  width: 100%;
  height: 35vh;
}

.slider1 {
  width: 100%;
  height: 100%;
  background: url('../assets/hooper/1.jpg');
  background-size: 100%;
}

.slider2 {
  width: 100%;
  height: 100%;
  background: url('../assets/hooper/2.jpg');
  background-size: 100%;
}

.slider3 {
  width: 100%;
  height: 100%;
  background: url('../assets/hooper/3.jpg');
  background-size: 100%;
}

.slider4 {
  width: 100%;
  height: 100%;
  background: url('../assets/hooper/4.jpg');
  background-size: 100%;
}

.slider5 {
  width: 100%;
  height: 100%;
  background: url('../assets/hooper/5.jpg');
  background-size: 100%;
}

.slider6 {
  width: 100%;
  height: 100%;
  background: url('../assets/hooper/6.jpg');
  background-size: 100%;
}
</style>