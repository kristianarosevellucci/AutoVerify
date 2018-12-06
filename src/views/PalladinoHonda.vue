<template>
  <div>
    <navigation />
    <div
      class="position-relative overflow-hidden p-3 p-md-5 m-md-3 text-center bg-light"
    >
      <div class="col-md-5 p-lg-5 mx-auto my-5">
        <h1 class="display-4 font-weight-normal">Palladino Honda</h1>
        <p class="lead font-weight-normal">
          That Car Place is to be used as a template for this page.
        </p>
        <a class="btn btn-outline-secondary" href="#">Coming soon</a>
      </div>
      <div class="product-device box-shadow d-none d-md-block"></div>
      <div
        class="product-device product-device-2 box-shadow d-none d-md-block"
      ></div>
    </div>

    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Navigation from './../components/navigation';
import Footer from './../components/footer';

export default {
  name: "palladino-honda",
  components: {
    Navigation,
    Footer
  }
};
</script>

<style>
.container {
  max-width: 960px;
}

/*
   * Custom translucent site header
   */

.site-header {
  background-color: rgba(0, 0, 0, 0.85);
  -webkit-backdrop-filter: saturate(180%) blur(20px);
  backdrop-filter: saturate(180%) blur(20px);
}
.site-header a {
  color: #999;
  transition: ease-in-out color 0.15s;
}
.site-header a:hover {
  color: #fff;
  text-decoration: none;
}

/*
   * Dummy devices (replace them with your own or something else entirely!)
   */

.product-device {
  position: absolute;
  right: 10%;
  bottom: -30%;
  width: 300px;
  height: 540px;
  background-color: #333;
  border-radius: 21px;
  -webkit-transform: rotate(30deg);
  transform: rotate(30deg);
}

.product-device::before {
  position: absolute;
  top: 10%;
  right: 10px;
  bottom: 10%;
  left: 10px;
  content: "";
  background-color: rgba(255, 255, 255, 0.1);
  border-radius: 5px;
}

.product-device-2 {
  top: -25%;
  right: auto;
  bottom: 0;
  left: 5%;
  background-color: #e5e5e5;
}

/*
   * Extra utilities
   */

.border-top {
  border-top: 1px solid #e5e5e5;
}
.border-bottom {
  border-bottom: 1px solid #e5e5e5;
}

.box-shadow {
  box-shadow: 0 0.25rem 0.75rem rgba(0, 0, 0, 0.05);
}

.flex-equal > * {
  -ms-flex: 1;
  -webkit-box-flex: 1;
  flex: 1;
}
@media (min-width: 768px) {
  .flex-md-equal > * {
    -ms-flex: 1;
    -webkit-box-flex: 1;
    flex: 1;
  }
}

.overflow-hidden {
  overflow: hidden;
}
</style>
