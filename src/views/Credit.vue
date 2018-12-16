<template>
    <Page>

    <tools-hero
      imageSrc="credit-hero.png"
      imageAlt="AutoVerify Credit"
      toolSubtitle="AutoVerify"
      toolTitle="Credit"
      toolDescription="Dealerships asked us to help them reduce costs. We listened."
      linkName="Watch Demo"
      class="tools-hero--maroon"
    />

    <introduction
      introductionText="Reduce your monthly spend by only running vehicle history reports on the vehicles that need it, not the ones that don’t. Only 30% of vehicles have accident history. Why buy costly history reports for 100% of your vehicles?"
    />

    <tool-benefits
      imageSrc="how-av-helps--credit.png"
      imageAlt="Screens"
      benefitsTitle="AutoVerify Credit Helps You:"
      benefitsNumber1="01"
      benefitsTitle1="Slash Costs"
      benefitsText1="You spend a small fortune on history reports every month. Accident Check lets you stay transparent while avoiding the expense of running reports on clean vehicles. Run your VINs through our system to discover which vehicles have accident history."
      benefitsNumber2="02"
      benefitsTitle2="Slash Costs"
      benefitsText2="You spend a small fortune on history reports every month. Accident Check lets you stay transparent while avoiding the expense of running reports on clean vehicles. Run your VINs through our system to discover which vehicles have accident history."
      benefitsNumber3="03"
      benefitsTitle3="Slash Costs"
      benefitsText3="You spend a small fortune on history reports every month. Accident Check lets you stay transparent while avoiding the expense of running reports on clean vehicles. Run your VINs through our system to discover which vehicles have accident history."
      benefitsNumber4="04"
      benefitsTitle4="Slash Costs"
      benefitsText4="You spend a small fortune on history reports every month. Accident Check lets you stay transparent while avoiding the expense of running reports on clean vehicles. Run your VINs through our system to discover which vehicles have accident history."
    />

    <tool-summary
      imageSrc="reports-placeholder.png"
      imageAlt="Screens"
      summaryTitle="It's true-- there's more to a history report than accident data. But..."
      summaryText="Why are you paying for information that's available for free?"
      bullet1="Recall status is available free online"
      bullet2="Odometer rollbacks can be detected by your service department"
      bullet3="Do buyers really care about registration history?"
    />

    <testimonials
      quote="“Our dealership got Mobials a few months ago, and we already have over 400 reviews! We just recently turned on the new Google feature and were able to move our Google ranking in a positive direction. I love the new feature that allows me to manage everything through one platform.”"
      author="Susan Gubasta"
      authorJob="President, TADA, Dealer Principal, Mississauga Toyota"
    />

    <cta-banner
      ctaText="Want to see it in action?"
      linkName="Watch Demo"
      class="cta-banner__maroon"
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
import ToolSummary from './../components/tool-summary';
import ToolBenefits from './../components/tool-benefits';
import ToolsHero from './../components/tools-hero';
import Testimonials from './../components/tools/testimonials';

export default {
  name: "Credit",
  components: {
    Introduction,
    CtaBanner,
    Page,
    Testimonials,
    ToolSummary,
    ToolBenefits,
    ToolsHero
  }
};
</script>

<style lang="scss">
  .divider {
    height: 5px;
    width: 50px;
    background: #E6E6E6;
    display: block;
    margin: 30px auto;
  }
</style>
