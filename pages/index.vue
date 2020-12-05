<template lang="pug">
  .wrapper
    .box1.flex
      h1.box1__title Long Beach Surfing Institute
      .box1__description Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.

    .box2.flex
      .box2__left
        .box2__title Recent Reviews
        .box2__description
          p Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed incididunt ut labore et dolore magn.
          .box2__author -  Steve Woz
        .box2__description
          p Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed incididunt ut labore et dolore magn.
          .box2__author -  Steve Woz
      .box2__main-video.flex
        img(src='images/video-main.png')
      .box2__right
        .box2__title User Videos
        img.box2__item-video(src='images/video-small.png')
        img.box2__item-video(src='images/video-small.png')

    .box3
      .box3__title Popular Instractors
      slider

    .box4
      .box4__title Recent Blogs by User
      .box4__row
        .box4__col-6
          div
            img(src='images/f1.png')
        .box4__col-6
          .box4__title2 Lipsum cound be headline
          .box4__description Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
          a.box4__btn(href="#") Read More
        .box4__col-6
          .box4__title2 Lipsum cound be headline
          .box4__description Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
          a.box4__btn(href="#") Read More
        .box4__col-6
          div
            img(src='images/f1.png')

    .box5
      .box5__title Aren’t you intrested Yet!!
      a.box5__btn(href="#") Enroll Now

</template>

<script>
import Slider from "@/components/slider/Slider";
export default {
  name: 'home',
  components: {
    Slider
  }
}
</script>

<style lang="sass">
  $fix-indent: 16px
  @mixin title
    font-size: 50px
    line-height: 56px
    text-align: center
    padding-bottom: 90px

  @mixin btn
    font-family: "Avenir"
    border: 1px solid #e5e5e5
    padding: 20px 30px

  .box1
    height: 580px
    flex-direction: column
    justify-content: center
    text-align: center

    .box1__title
      font-size: 70px
      line-height: 76px

    .box1__description
      margin-top: 25px
      color: #999999
      padding: 0 400px

  .box2
    justify-content: space-between
    margin-bottom: 230px

    .box2__left, .box2__right
      display: flex
      flex-direction: column
      justify-content: space-between
      flex: 0 1 280px
    .box2__left
      padding-left: $fix-indent
    .box2__title
      font-size: 36px
      line-height: 42px
      margin-top: 20px
    .box2__description
      background: url(../static/img/quote.png) no-repeat 0 0
      padding-left: $fix-indent
      margin-left: -$fix-indent
      border-bottom: 1px solid #e7e7e7
      padding-bottom: 20px
    .box2__description p
      font-family: avenir-book-oblique
      color: #999999
    .box2__author
      padding-top: 20px
    .box2__main-video
      flex: 1 0 auto
      justify-content: center
      align-items: flex-start
    .box2__item-video
      align-self: center
      width: 100%
      height: auto

  .box3
    margin-bottom: 200px

    .box3__title
      @include title

  .box4
    margin: 0 auto
    max-width: 1050px

    .box4__title
      @include title
    .box4__row
      margin: 0 -40px
      display: flex
      flex-wrap: wrap
    .box4__col-6
      width: 50%
      padding: 0 40px
      margin-bottom: 90px
    img
      width: 100%
      max-width: 100%
      display: block
    .box4__title2
      font-style: italic
      font-size: 40px
      line-height: 46px
      margin: 40px 0 30px
    .box4__description
      color: #444444
      margin-bottom: 45px
    .box4__btn
      @include btn

  .box5
    text-align: center
    margin-top: 170px
    margin-bottom: 145px
    .box5__title
      @include title
    .box5__btn
      @include btn
</style>
