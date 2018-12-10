<template>
  <Page>

  <tools-hero
    imageSrc="tradein-hero.png"
    imageAlt="AutoVerify Trade-in"
    toolSubtitle="AutoVerify"
    toolTitle="Trade-in"
    toolDescription="More leads. Better leads. Even on mobile."
    linkName="Watch Demo"
    class="tools-hero--pink"
  />

  <introduction
    introductionText="Consumers are online looking for their trade-in value. Give them the information they want from an unbiased third party they know and trust."
    />

  <tool-benefits
    imageSrc="help-placeholder.png"
    imageAlt="Screens"
    benefitsTitle="AutoVerify Trade-in Helps You:"
    benefitsNumber1="01"
    benefitsTitle1="Trade-ins + Credit apps = win-win"
    benefitsText1="A trade-in value tool is the highest lead-generating tool on your site. AutoVerify Trade-in lets you generate credit-qualified leads and credit applications from consumers looking for trade-in values."
    benefitsNumber2="02"
    benefitsTitle2="Satisfy Customers"
    benefitsText2="Create a user-friendly experience with the info they want in the format they want it. No waiting, no follow-ups — just a simple, mobile-optimized value range delivered on command."
    benefitsNumber3="03"
    benefitsTitle3="Integrate Easily"
    benefitsText3="Integrates seamlessly with your website and online listings. Maximize the value of your VDPs by loading them with info that solves uncertainty about the purchase process."
    benefitsNumber4="04"
    benefitsTitle4="Be Chosen"
    benefitsText4="Differentiate yourself with transparent info that answers your customer's questions without trying to sell. Earn the lead with valuable information, then nurture it until they’re ready to buy."
  />

  <tool-summary
    imageSrc="reports-placeholder.png"
    imageAlt="Screens"
    summaryTitle="It's true-- there's more to a history report than accident data. But..."
    summaryText=" "
    bullet1="Customized, downloadable report"
    bullet2="Simple CRM integrations"
    bullet3="No long forms to complete"
  />

  <testimonials
    quote="“Mobials has been very prompt at getting things done and has been very helpful anytime I have had questions or need anything done at all.  Super easy to work with.”"
    author="Hutch Orr"
    authorJob="Auto Worx"
  />

  <tools-cta-banner
    ctaText="Want to see it in action?"
    linkName="Watch Demo"
    class="cta-banner__pink"
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
  name: "contact",
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
