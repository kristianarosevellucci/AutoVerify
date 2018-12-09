<template>
  <section class="tool-summary">
    <div class="container-fluid">
      <div class="row">
        <div class="col-sm-6">
          <img
            :src="require(`@/../public/img/tools/${imageSrc}`)"
            :alt="imageAlt"
            class="img-responsive"
          />
        </div>
        <div class="offset-sm-1 col-sm-5">
          <h2>{{summaryTitle}}</h2>
          <ul class="tool-summary__list">
            <li>{{bullet1}}</li>
            <li>{{bullet2}}</li>
            <li>{{bullet3}}</li>
          </ul>
          <p>{{summaryText}}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: "ToolSummary",
    props: {
      imageSrc: {
        type: String,
        required: true
      },
      imageAlt: {
        type: String,
        required: true
      },
      summaryTitle: {
        type: String,
        required: true
      },
      summaryText: {
        type: String,
        required: true
      },
      bullet1: {
        type: String,
        required: true
      },
      bullet2: {
        type: String,
        required: true
      },
      bullet3: {
        type: String,
        required: true
      },
    }
  }
</script>

<style lang="scss" scoped>
  @import "../../public/scss/application.scss";
  p {
    font-size: 14px;
  }
</style>
