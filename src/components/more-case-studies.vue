<template>
  <div class="more-case-studies text-center">
      <div class="container-fluid">
        <div class="row">
          <div class="col-sm-12">
            <h2 class="more-case-studies__title">{{sectionTitle}}</h2>
          </div>
        </div>
        <div class="more-case-studies__content">
          <div class="row">
            <div class="col-sm-3">
              <router-link class=“more-case-studies__item” to=“/”>
                <div class="more-case-studies__img">
                  <img
                    :src="require(`@/../public/img/${imageSrc1}`)"
                    :alt="imageAlt1"
                    class="img-responsive"
                  />
                </div>
                <div class="case-study-content text-left">
                  <h3 class="case-study-content__title">{{wheatonChevrolet}}</h3>
                  <p class="case-study-content__link">{{viewCaseStudy}}</p>
                </div>
              </router-link>
            </div>
            <div class="col-sm-3">
              <router-link class=“more-case-studies__item” to=“/”>
                <div class="more-case-studies__img">
                  <img
                    :src="require(`@/../public/img/${imageSrc2}`)"
                    :alt="imageAlt2"
                    class="img-responsive"
                  />
                </div>
                <div class="case-study-content text-left">
                  <h3 class="case-study-content__title">{{palladinoHonda}}</h3>
                  <p class="case-study-content__link">{{viewCaseStudy}}</p>
                </div>
              </router-link>
            </div>
            <div class="col-sm-3">
              <router-link class=“more-case-studies__item” to=“/”>
                <div class="more-case-studies__img">
                  <img
                    :src="require(`@/../public/img/${imageSrc3}`)"
                    :alt="imageAlt3"
                    class="img-responsive"
                  />
                </div>
                <div class="case-study-content text-left">
                  <h3 class="case-study-content__title">{{goAuto}}</h3>
                  <p class="case-study-content__link">{{viewCaseStudy}}</p>
                </div>
              </router-link>
            </div>
            <div class="col-sm-3">
              <router-link class=“more-case-studies__item” to=“/”>
                <div class="more-case-studies__img">
                  <img
                    :src="require(`@/../public/img/${imageSrc1}`)"
                    :alt="imageAlt1"
                    class="img-responsive"
                  />
                </div>
                <div class="case-study-content text-left">
                  <h3 class="case-study-content__title">{{thatCarPlace}}</h3>
                  <p class="case-study-content__link">{{viewCaseStudy}}</p>
                </div>
              </router-link>
            </div>
          </div>
        </div>
      </div>
  </div>
</template>

<script>
  export default {
    name: "MoreCaseStudies",
    props: {
      imageSrc1: {
        type: String,
        required: true
      },
      imageAlt1: {
        type: String,
        required: true
      },
      imageSrc2: {
        type: String,
        required: true
      },
      imageAlt2: {
        type: String,
        required: true
      },
      imageSrc3: {
        type: String,
        required: true
      },
      imageAlt3: {
        type: String,
        required: true
      },
      imageSrc4: {
        type: String,
        required: true
      },
      imageAlt4: {
        type: String,
        required: true
      },
      sectionTitle: {
        type: String,
        required: true
      },
      wheatonChevrolet: {
        type: String,
        required: true
      },
      thatCarPlace: {
        type: String,
        required: true
      },
      goAuto: {
        type: String,
        required: true
      },
      palladinoHonda: {
        type: String,
        required: true
      },
      viewCaseStudy: {
        type: String,
        required: true
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "../../public/scss/application.scss";
</style>
