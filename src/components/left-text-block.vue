<template>
  <div class="text-block">
    <div class="container">
      <div class="row">
        <div class="offset-md-1 col-md-5">
          <p class="text-block__inline-testimonial">{{inlineTestimonial1}}</p>
          <p class="text-block__text">{{textBlock1}}</p>
          <p class="text-block__inline-testimonial">{{inlineTestimonial2}}</p>
          <p class="text-block__text">{{textBlock2}}</p>
          <router-link class=“btn-primary” to=“/”>{{linkName}}</router-link>
        </div>
        <div class="col-md-6">
          <img
            :src="require(`@/../public/img/${imageSrc}`)"
            :alt="imageAlt"
            class="img-responsive"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "LeftTextBlock",
    props: {
      inlineTestimonial1: {
        type: String,
        required: true
      },
      textBlock1: {
        type: String,
        required: true
      },
      inlineTestimonial2: {
        type: String,
        required: true
      },
      textBlock2: {
        type: String,
        required: true
      },
      linkName: {
        type: String,
        required: true
      },
      imageSrc: {
        type: String,
        required: true
      },
      imageAlt: {
        type: String,
        required: true
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "../../public/scss/application.scss";
</style>
