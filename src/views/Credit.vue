<template>
    <Page>
    <section class="hero">
      <div class="container-fluid">
        <div class="row">
          <div class="col-sm-5">
            <p>AutoVerify</p>
            <h1>Accident Check</h1>
            <p>Dealerships asked us to help them reduce costs. We listened.</p>
            <a href="#" class="btn-primary">Watch Demo</a>
          </div>
          <div class="col-sm-7">
            <img src="#" alt="Screen">
          </div>
        </div>
      </div>

    </section>

    <introduction
      introductionText="Reduce your monthly spend by only running vehicle history reports on the vehicles that need it, not the ones that don’t. Only 30% of vehicles have accident history. Why buy costly history reports for 100% of your vehicles?"
    />

    <section class="how-it-helps">
      <div class="container-fluid">
        <div class="row">
          <div class="col-sm-3">
            <img src="#" alt="Featured Image">
          </div>
          <div class="col-sm-9">
            <div class="row">
              <div class="col-sm-12">
                <h2>Accident Check Helps You:</h2>
              </div>
            </div>
            <div class="row">
              <div class="col-sm-6">
                <h3><span class="how-it-helps__number">01</span>Slash Costs</h3>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <statistics
      statNumber1="30"
      statNumber2="5"
      statNumber3="189"
      statTitle1="Credit Leads"
      statTitle2="Insurance Leads"
      statTitle3="Trade-in Leads"
      statisticsTitle="Monthly Average Lead Generation"
    />

    <ctaBanner
      ctaText="Want to learn more about this story?"
      linkName="Contact Us"
      class="cta-banner__palladino"
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

    </Page>
</template>

<script>
// @ is an alias to /src
import Page from './../components/page';
import Introduction from './../components/introduction';
import LeftTextBlock from './../components/left-text-block';
import RightTextBlock from './../components/right-text-block';
import Statistics from './../components/statistics';
import CtaBanner from './../components/cta-banner';
import MoreCaseStudies from './../components/more-case-studies';

export default {
  name: "contact",
  components: {
    Introduction,
    LeftTextBlock,
    RightTextBlock,
    Statistics,
    CtaBanner,
    MoreCaseStudies,
    Page
  }
};
</script>

<style></style>
