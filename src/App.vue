<template>
  <div id="app">
    <router-view />
    <Footer
      poweredBy="Powered by "
      footerCenterText="192 Dundas St Suite 300 | London, ON N6A 1G7 | Tel: 1.877.833.1423"
      copyRight="Copyright 2019. All rights reserved."
    />
  </div>
</template>

<script>
// @ is an alias to /src
import Footer from './components/footer';

export default {
  name: "that-car-place",
  components: {
    Footer
  }
};
</script>


<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "../public/scss/application.scss";
@import url('https://fonts.googleapis.com/css?family=Cairo:400,600,700|Montserrat:400,700,800');
</style>
