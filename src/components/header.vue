<template>
    <header>
      <div class="header-container container-fluid">
        <div class="content-container">
          <div class="header-cta-container">
            <img
              :src="require(`@/../public/img/logo.svg`)"
              :alt="imageAlt"
              class="header-logo"
            />
            <button class="menuToggle" @click="$emit('toggleNavigation')">
              <span class="menuIcon">
                <span></span>
                <span></span>
              </span>
            </button>
          </div>
        </div>
      </div>
      <div class="navigation">
        <div class="container-fluid">
          <div class="navigation-content">
            <div class="row">
              <div class="hidden-xs hidden-sm col-md-5">
                <h2>Reduce Costs. Increase Sales. Satisfy Customers.</h2>
                <router-link exact to=“/”>LinkedIn</router-link>
                <router-link exact to=“/”>Facebook</router-link>
                <router-link exact to=“/”>Instagram</router-link>
                <router-link exact to=“/”>Youtube</router-link>
                <router-link exact to=“/”>Twitter</router-link>
              </div>
              <div class="col-sm-4 offset-md-1 col-md-2">
                <router-link exact to=“/” @click.native="$emit('closeNavigation')" class="navigation__section-title">Home</router-link>
                <div class="navigation__link-group">
                  <router-link exact to=“/” @click.native="$emit('closeNavigation')" class="navigation__section-title">Products</router-link>
                  <ul class="navigation__group-items">
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')" class="">Credit</router-link></li>
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">Reviews</router-link></li>
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">Total Loss</router-link></li>
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">Insurance</router-link></li>
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">ReserveNow</router-link></li>
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">Trade-in</router-link></li>
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">Accident Check (beta)</router-link></li>
                  </ul>
                </div>
              </div>
              <div class="col-sm-4 col-md-2">
                <router-link exact to=“/” @click.native="$emit('closeNavigation')" class="navigation__section-title">How It Works</router-link>
                <div class="navigation__link-group">
                  <router-link exact to=“/” @click.native="$emit('closeNavigation')" class="navigation__section-title">Pricing</router-link>
                </div>
                <div class="navigation__link-group">
                  <router-link exact to=“/” @click.native="$emit('closeNavigation')" class="navigation__section-title">Customers</router-link>
                  <ul class="navigation__group-items">
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">Wheaton Chevrolet</router-link></li>
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">Palladino Honda</router-link></li>
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">That Car Place</router-link></li>
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">Go Auto Outlets</router-link></li>
                  </ul>
                </div>
              </div>
              <div class="col-sm-4 col-md-2">
                  <router-link exact to=“/” @click.native="$emit('closeNavigation')" class="navigation__section-title">About Us</router-link>
                <div class="navigation__link-group">
                  <router-link exact to=“/” @click.native="$emit('closeNavigation')" class="navigation__section-title">Company</router-link>
                  <ul class="navigation__group-items">
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">Terms &amp; Conditions</router-link></li>
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">Privacy Policy</router-link></li>
                    <li class="navigation__sublink"><router-link exact to=“/” @click.native="$emit('closeNavigation')">Contact Us</router-link></li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    imageSrc: {
      type: String,
      required: true
    },
    imageAlt: {
      type: String,
      required: true
    }
  }
};
</script>
