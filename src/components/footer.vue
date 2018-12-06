<template>
    <footer class="container-fluid py-2">
      <div class="row">
        <div class="col-sm-3">
          <p>{{poweredBy}}</p>
        </div>
        <div class="col-sm-6 text-center">
          <p>{{footerCenterText}}</p>
        </div>
        <div class="col-sm-3">
          <p class="text-right">{{copyRight}}</p>
        </div>
      </div>
    </footer>
</template>

<script>
  export default {
    name: "Footer",
    props: {
      footerCenterText: {
        type: String,
        required: true
      },
      poweredBy: {
        type: String,
        required: true
      },
      copyRight: {
        type: String,
        required: true
      }
    }
  }
</script>

<style lang="scss" scoped>
  $red: #ff0000;

  p {
    font-family: 'Cairo', sans-serif;
    font-size: 14px;
    color: $red;
  }
</style>
