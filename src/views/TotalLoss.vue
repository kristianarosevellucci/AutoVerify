<template>
  <Page>

  <tools-hero
    imageSrc="credit-hero.png"
    imageAlt="AutoVerify Insurance"
    toolSubtitle="AutoVerify"
    toolTitle="Total Loss"
    toolDescription="Earn quality leads from customers that have wrecked a car and need a new one."
    linkName="Watch Demo"
  />

  <introduction
    introductionText="Provide them with documentation to use in their insurance negotiations and build trust by helping them get more money for their wrecked car."
    />

  <tool-benefits
    imageSrc="help-placeholder.png"
    imageAlt="Screens"
    benefitsTitle="AutoVerify Total Loss Helps You:"
    benefitsNumber1="01"
    benefitsTitle1="High-Quality Leads"
    benefitsText1="A person with a vehicle damaged beyond repair needs a replacement vehicle, and they need it now. Total Loss Reports give you a high-converting lead that is ready to buy. "
    benefitsNumber2="02"
    benefitsTitle2="Build Trust"
    benefitsText2="Be the one who gives them peace-of-mind about their insurance offer, and let them know they can trust you to help them through the purchase of a new vehicle."
    benefitsNumber3="03"
    benefitsTitle3="Get Them More Money"
    benefitsText3="Help customers get more for their wrecked car, so they turn to you for a replacement."
    benefitsNumber4="04"
    benefitsTitle4="Optimized for Mobile"
    benefitsText4="AutoVerify tools are designed and optimized for mobile, so when your customers get their information, it’s formatted to fit the device they’re using."
  />

  <tool-summary
    imageSrc="reports-placeholder.png"
    imageAlt="Screens"
    summaryTitle="It's true-- there's more to a history report than accident data. But..."
    summaryText=" "
    bullet1="Customer wrecks their car and receives a settlement offer"
    bullet2="They receive a Total Loss Report"
    bullet3="They use report in settlement negotiations and get more money"
  />

  <testimonials
    quote="“Mobials has been very prompt at getting things done and has been very helpful anytime I have had questions or need anything done at all.  Super easy to work with.”"
    author="Hutch Orr"
    authorJob="Auto Worx"
  />

  <tools-cta-banner
    ctaText="Want to see it in action?"
    linkName="Watch Demo"
    class="cta-banner__palladino"
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
import ToolsCtaBanner from './../components/tools/tools-cta-banner';
import Testimonials from './../components/tools/testimonials';

export default {
  name: "TotalLoss",
  components: {
    Introduction,
    CtaBanner,
    Page,
    ToolsCtaBanner,
    Testimonials,
    ToolSummary,
    ToolBenefits,
    ToolsHero
  }
};
</script>

<style>
  .divider {
    height: 5px;
    width: 50px;
    background: #E6E6E6;
    display: block;
    margin: 30px auto;
  }
</style>
