<template>
  <div id="app">
    <router-view />
    <Footer
      poweredBy="Powered by Mobials"
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
</style>
