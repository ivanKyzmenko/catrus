<template>
  <div id="app">
    <!--<img alt="Vue logo" src="./assets/logo.png">-->
    <MainHeader></MainHeader>

    <Carousel></Carousel>

    <div class="catrus-custom container">
      <div class="container-fit">
        <h1 class="catrus-custom__title">Your Custom Essay and Term Paper Writing Assistant</h1>
        <h3 class="catrus-custom__subtitle text-with-line">A Turnkey Writing Service Solution For Any Project</h3>

        <div class="catrus-custom__data">
            <h2 class="catrus-custom__data-title">
              <span class="catrus-custom__data-title__orange">Meister</span> is a German word for master or highly skilled and knowledgeable specialist. </h2>
            <span class="catrus-custom__data-text">Hence, the name Customessaymeister. We&apos;ve been doing academic writing, ghostwriting and freelance writing since 2006, when the website was first crafted by our entrepreneurial founder. We are not an on-line flea market with hundreds of writers&apos; profiles/avatars - <b>we are a real company that offers a turnkey, hands-off custom writing solution to your need!</b></span>
        </div>
      </div>

      <div class="catrus-custom__bottom">
        <div class="container-fit">
          <div class="catrus-custom__bottom-text">With us, you get great fully managed freelance writers that are backed by a full time team of project managers who are on standby 24/7 to make sure your project is done the right way!</div>
          <div class="catrus-custom__bottom-img">
            <img src="./assets/custom.png" alt="">
          </div>

        </div>
      </div>
    </div>

    <Service></Service>
    <HowWeWork></HowWeWork>
    <Reviews></Reviews>
    <MainFooter></MainFooter>
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue'
import Carousel from './components/carousel/Carousel.vue'
import Service from './components/service/OurService.vue'
import HowWeWork from './components/how-we-work/HowWeWork.vue'
import Reviews from './components/reviews/Reviews.vue'

import MainFooter from './components/MainFooter.vue'

export default {
  name: 'CatrusApp',
  components: {
    MainHeader,
    Carousel,
    MainFooter,
    Service,
    HowWeWork,
    Reviews
  }
}
</script>

<style lang="scss">
  @import "./scss/main";
</style>
