<template>
    <header>
      <div class="header-container container-fluid">
        <div class="content-container">
          <div class="header-cta-container">
            <router-link to="/">
              <img
                :src="require(`@/../public/img/logo.svg`)"
                :alt="imageAlt"
                class="header-logo"
              />
            </router-link>
            <router-link class="btn-primary header-btn" to=“/”>Book Demo</router-link>
            <button class="menuToggle" @click="$emit('toggleNavigation')">
              <span class="menuIcon">
                <span></span>
                <span></span>
                <span></span>
              </span>
            </button>
            <div class="dropdown">
              <button class="dropdown-toggle lang-dropdown" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                <img
                  :src="require(`@/../public/img/canadian-flag.svg`)"
                  :alt="imageAlt"
                  class="lang-flag"
                />
                <span class="lang-text">ENG</span>
              </button>
              <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                <a class="lang-dropdown-item lang-text" href="#">
                  <img
                    :src="require(`@/../public/img/canadian-flag.svg`)"
                    :alt="imageAlt"
                    class="lang-flag"
                  />
                  FR
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="navigation">
        <div class="container-fluid">
          <div class="navigation-content">
            <div class="row">
              <div class="hidden-xs hidden-sm col-md-5">
                <div class="row">
                  <div class="col-md-12">
                    <p class="navigation__dropdown-text">Reduce Costs. <br> Increase Sales. <br> Satisfy Customers.</p>
                  </div>
                </div>
                <div class="row">
                  <div class="col-md-12">
                    <router-link exact to=“/” class="social-media clip-circle">
                      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" id="linkedin"><path id="linkedin-bg" d="M12 0c-6.627 0-12 5.373-12 12s5.373 12 12 12 12-5.373 12-12-5.373-12-12-12zm-2 16h-2v-6h2v6zm-1-6.891c-.607 0-1.1-.496-1.1-1.109 0-.612.492-1.109 1.1-1.109s1.1.497 1.1 1.109c0 .613-.493 1.109-1.1 1.109zm8 6.891h-1.998v-2.861c0-1.881-2.002-1.722-2.002 0v2.861h-2v-6h2v1.093c.872-1.616 4-1.736 4 1.548v3.359z"/></svg>
                    </router-link>
                    <router-link exact to=“/” class="social-media">
                      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" id="facebook"><path id="facebook-bg" d="M12 0c-6.627 0-12 5.373-12 12s5.373 12 12 12 12-5.373 12-12-5.373-12-12-12zm3 8h-1.35c-.538 0-.65.221-.65.778v1.222h2l-.209 2h-1.791v7h-3v-7h-2v-2h2v-2.308c0-1.769.931-2.692 3.029-2.692h1.971v3z"/></svg>
                    </router-link>
                    <router-link exact to=“/” class="social-media">
                      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" id="instagram"><path id="instagram-bg" d="M14.829 6.302c-.738-.034-.96-.04-2.829-.04s-2.09.007-2.828.04c-1.899.087-2.783.986-2.87 2.87-.033.738-.041.959-.041 2.828s.008 2.09.041 2.829c.087 1.879.967 2.783 2.87 2.87.737.033.959.041 2.828.041 1.87 0 2.091-.007 2.829-.041 1.899-.086 2.782-.988 2.87-2.87.033-.738.04-.96.04-2.829s-.007-2.09-.04-2.828c-.088-1.883-.973-2.783-2.87-2.87zm-2.829 9.293c-1.985 0-3.595-1.609-3.595-3.595 0-1.985 1.61-3.594 3.595-3.594s3.595 1.609 3.595 3.594c0 1.985-1.61 3.595-3.595 3.595zm3.737-6.491c-.464 0-.84-.376-.84-.84 0-.464.376-.84.84-.84.464 0 .84.376.84.84 0 .463-.376.84-.84.84zm-1.404 2.896c0 1.289-1.045 2.333-2.333 2.333s-2.333-1.044-2.333-2.333c0-1.289 1.045-2.333 2.333-2.333s2.333 1.044 2.333 2.333zm-2.333-12c-6.627 0-12 5.373-12 12s5.373 12 12 12 12-5.373 12-12-5.373-12-12-12zm6.958 14.886c-.115 2.545-1.532 3.955-4.071 4.072-.747.034-.986.042-2.887.042s-2.139-.008-2.886-.042c-2.544-.117-3.955-1.529-4.072-4.072-.034-.746-.042-.985-.042-2.886 0-1.901.008-2.139.042-2.886.117-2.544 1.529-3.955 4.072-4.071.747-.035.985-.043 2.886-.043s2.14.008 2.887.043c2.545.117 3.957 1.532 4.071 4.071.034.747.042.985.042 2.886 0 1.901-.008 2.14-.042 2.886z"/></svg>
                    </router-link>
                    <router-link exact to=“/” class="social-media">
                      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" id="twitter"><path id="twitter-bg" d="M12 0c-6.627 0-12 5.373-12 12s5.373 12 12 12 12-5.373 12-12-5.373-12-12-12zm6.066 9.645c.183 4.04-2.83 8.544-8.164 8.544-1.622 0-3.131-.476-4.402-1.291 1.524.18 3.045-.244 4.252-1.189-1.256-.023-2.317-.854-2.684-1.995.451.086.895.061 1.298-.049-1.381-.278-2.335-1.522-2.304-2.853.388.215.83.344 1.301.359-1.279-.855-1.641-2.544-.889-3.835 1.416 1.738 3.533 2.881 5.92 3.001-.419-1.796.944-3.527 2.799-3.527.825 0 1.572.349 2.096.907.654-.128 1.27-.368 1.824-.697-.215.671-.67 1.233-1.263 1.589.581-.07 1.135-.224 1.649-.453-.384.578-.87 1.084-1.433 1.489z"/></svg>
                    </router-link>
                  </div>
                </div>
                <div class="row">
                  <div class="col-md-12">
                    <router-link class="btn-primary mobile-demo-btn" to=“/”>Book Demo</router-link>
                  </div>
                </div>
              </div>
              <div class="col-sm-4 offset-md-1 col-md-2">
                <router-link exact to="/" @click.native="$emit('closeNavigation')" class="navigation__section-title">Home</router-link>
                <div class="navigation__link-group">
                  <router-link exact to="/tools/credit" @click.native="$emit('closeNavigation')" class="navigation__section-title">Products</router-link>
                  <ul class="navigation__group-items">
                    <li class="navigation__sublink"><router-link exact to="/tools/credit" @click.native="$emit('closeNavigation')" class="">Credit</router-link></li>
                    <li class="navigation__sublink"><router-link exact to="/tools/reviews" @click.native="$emit('closeNavigation')">Reviews</router-link></li>
                    <li class="navigation__sublink"><router-link exact to="/tools/total-loss" @click.native="$emit('closeNavigation')">Total Loss</router-link></li>
                    <li class="navigation__sublink"><router-link exact to="/tools/insurance" @click.native="$emit('closeNavigation')">Insurance</router-link></li>
                    <li class="navigation__sublink"><router-link exact to="/tools/reserve-now" @click.native="$emit('closeNavigation')">ReserveNow</router-link></li>
                    <li class="navigation__sublink"><router-link exact to="/tools/trade-in" @click.native="$emit('closeNavigation')">Trade-in</router-link></li>
                    <li class="navigation__sublink"><router-link exact to="/tools/accident-check" @click.native="$emit('closeNavigation')">Accident Check (beta)</router-link></li>
                  </ul>
                </div>
              </div>
              <div class="col-sm-4 col-md-2">
                <router-link exact to=“/” @click.native="$emit('closeNavigation')" class="navigation__section-title">How It Works</router-link>
                <div class="navigation__link-group">
                  <router-link exact to="/customers/wheaton-chevrolet" @click.native="$emit('closeNavigation')" class="navigation__section-title">Customers</router-link>
                  <ul class="navigation__group-items">
                    <li class="navigation__sublink"><router-link exact to="/customers/wheaton-chevrolet" @click.native="$emit('closeNavigation')">Wheaton Chevrolet</router-link></li>
                    <li class="navigation__sublink"><router-link exact to="/customers/palladino-honda" @click.native="$emit('closeNavigation')">Palladino Honda</router-link></li>
                    <li class="navigation__sublink"><router-link exact to="/customers/that-car-place" @click.native="$emit('closeNavigation')">That Car Place</router-link></li>
                    <li class="navigation__sublink"><router-link exact to="/customers/go-auto-outlets" @click.native="$emit('closeNavigation')">Go Auto Outlets</router-link></li>
                  </ul>
                </div>
              </div>
              <div class="col-sm-4 col-md-2">
                  <router-link exact to="/about" @click.native="$emit('closeNavigation')" class="navigation__section-title">About Us</router-link>
                <div class="navigation__link-group">
                  <router-link exact to="/" @click.native="$emit('closeNavigation')" class="navigation__section-title">Company</router-link>
                  <ul class="navigation__group-items">
                    <li class="navigation__sublink"><router-link exact to="/" @click.native="$emit('closeNavigation')">Terms &amp; Conditions</router-link></li>
                    <li class="navigation__sublink"><router-link exact to="/" @click.native="$emit('closeNavigation')">Privacy Policy</router-link></li>
                    <li class="navigation__sublink"><router-link exact to="/contact" @click.native="$emit('closeNavigation')">Contact Us</router-link></li>
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

<style scoped lang="scss">
  .btn-primary {
    margin-right: 20px;
  }
</style>
