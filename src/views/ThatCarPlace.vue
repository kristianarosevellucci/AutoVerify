<template>
  <div>
    <navigation />
    <div
      class="position-relative overflow-hidden p-3 p-md-5 m-md-3 text-center bg-light"
    >
        <h1>That Car Place</h1>
    </div>

    <introduction
      introductionText="Kal looked to Mobials' suite of tools to help him achieve his dream of 'an Amazon-like experience', where consumers could do all their pre-purchase research online, from reviews to values to credit approval, and even complete the sale."
    />

    <left-text-block class="top-block"
      inlineTestimonial1="Testimonial 1"
      textBlock1="Text block 1"
      inlineTestimonial2="Testimonial 2"
      textBlock2="Text block 2"
      linkName="Home"
      imageSrc="that-car-place-1.png"
      imageAlt="Screens"
    />

    <right-text-block class="bottom-block"
      inlineTestimonial1="Testimonial 1"
      textBlock1="Text block 1"
      inlineTestimonial2="Testimonial 2"
      textBlock2="Text block 2"
      linkName="Home"
      imageSrc="that-car-place-2.png"
      imageAlt="Screens"
    />

    <statistics
      statNumber1="75"
      statNumber2="14"
      statNumber3="168"
      statTitle1="Screens"
      statTitle2="Screens"
      statTitle3="Screens"
      statisticsSubtitle="Screens"
      statisticsTitle="Screens"
    />

    <ctaBanner
      ctaText="ctaText"
      linkName="linkName"
    />

    <MoreCaseStudies
    sectionTitle="Read More Case Studies"
    imageSrc1="case-study-placeholder.png"
    imageAlt1="Screens"
    imageSrc2="case-study-placeholder.png"
    imageAlt2="Screens"
    imageSrc3="case-study-placeholder.png"
    imageAlt3="Screens"
    imageSrc4="case-study-placeholder.png"
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
import Navigation from './../components/navigation';
import Introduction from './../components/introduction';
import LeftTextBlock from './../components/left-text-block';
import RightTextBlock from './../components/right-text-block';
import Statistics from './../components/statistics';
import CtaBanner from './../components/cta-banner';
import MoreCaseStudies from './../components/more-case-studies';
import Footer from './../components/footer';

export default {
  name: "that-car-place",
  components: {
    Navigation,
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

<style></style>
