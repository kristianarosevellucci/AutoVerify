<template>
  <div>
    <div class="position-relative overflow-hidden p-3 p-md-5 m-md-3 text-center bg-light">
        <h1>Go Auto Outlets</h1>
    </div>

    <introduction
      introductionText="AutoVerify tools have become a cornerstone of Go Auto Outlet’s lead generation strategy because they don’t just generate leads — they generate leads that convert into appointments and sales. "
    />

    <left-text-block class="top-block"
      textBlock1="That’s why, when the Mobials team approached them to discuss their ground-breaking new digital retailing solutions, Casey Pilip, Director of Business Development for Go Auto Outlet’s three locations, was quick to give it a try. They integrated AutoVerify Trade-in and Credit widgets to generate highly-qualified leads and provide consumers with valuable information to help with their search. While all three tools were helpful, Go Auto was blown away by the near-instant success they saw with the Credit tool."
      imageSrc="goauto-1.png"
      imageAlt="Go Auto Widgets"
    />

    <statistics
      statNumber1="32"
      statNumber2="14"
      statNumber3="9"
      statTitle1="Leads"
      statTitle2="Showroom Appointments"
      statTitle3="Cars Sold"
      statisticsSubtitle="After 30 Days of Using AutoVerify Credit,"
      statisticsTitle="Go Auto Outlets Recieved:"
    />

    <right-text-block class="pb-200"
      textBlock1="Because of the success Go Auto Outlets have had with AutoVerify Trade-in and Credit tools, Pilip is looking forward to experimenting with more digital retailing value-for-value tools like AutoVerify Insurance and Reserve Now. “Mobials is always creating new tools and innovating on the existing ones, so I love being one of the first one to leverage them all”."
      imageSrc="goauto-2.png"
      imageAlt="Screens"
    />

    <ctaBanner
      ctaText="Want to Learn More About This Story?"
      linkName="Contact Us"
      class="cta-banner__go-auto"
    />

    <MoreCaseStudies
    sectionTitle="Read More Case Studies"
    imageSrc1="related-cases-wheaton.png"
    imageAlt1="Screens"
    imageSrc2="related-cases-palladino.png"
    imageAlt2="Screens"
    imageSrc3="related-cases-goauto.png"
    imageAlt3="Screens"
    imageSrc4="related-cases-carplace.png"
    imageAlt4="Screens"
    wheatonChevrolet="Wheaton Chevrolet"
    thatCarPlace="That Car Place"
    palladinoHonda="Palladino Honda"
    goAuto="Go Auto Outlets"
    viewCaseStudy="View Case Study"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import Introduction from './../components/introduction';
import LeftTextBlock from './../components/left-text-block';
import RightTextBlock from './../components/right-text-block';
import Statistics from './../components/statistics';
import CtaBanner from './../components/cta-banner';
import MoreCaseStudies from './../components/more-case-studies';
import Footer from './../components/footer';

export default {
  name: "go-auto-outlets",
  components: {
    Footer,
    Introduction,
    LeftTextBlock,
    RightTextBlock,
    Statistics,
    CtaBanner,
    MoreCaseStudies,
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
