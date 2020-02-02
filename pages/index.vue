<template>
  <div class="p-Home">
    <Hero />

    <StatsBlock>
      The total amount of residential <br />
      transations has increasd by 22% <br />
      over the last year in Toronto.
    </StatsBlock>

    <ContentBlock background="#314259" color="#fff" sectionName="s-Buying">
      <template #title>
        <h2>Buying</h2>
      </template>
      <template #content>
        <p>
          We understand that buying a property in Toronto can be tough, let us
          help you with our expertise and knowledge for your next big purchase.
          We want you to buy a home that you can afford and love, no compromise.
        </p>
        <div class="p-Home_ButtonsWrap">
          <button class="g-Button">Book a Consultation</button>
          <button class="g-Button">Get your free buyers guide</button>
        </div>
      </template>
      <template #svg>
        <BuyingSVG />
      </template>
    </ContentBlock>

    <StatsBlock>
      The total amount of residential <br />
      transations has increasd by 22% <br />
      over the last year in Toronto.
    </StatsBlock>

    <ContentBlock background="#4A5460" color="#fff" sectionName="s-Selling">
      <template #title>
        <h2>Selling</h2>
      </template>
      <template #content>
        <p>
          List your home with us at <strong><em>1.5% comission rate</em></strong
          >. <br />
          With real data and numbers, we can help sell your home at the price
          you want, when you want.
        </p>
        <div class="p-Home_ButtonsWrap">
          <button class="g-Button">Book a Home Evaluation</button>
          <button class="g-Button">Get your free sellers guide</button>
        </div>
      </template>
      <template #svg>
        <SellingSVG />
      </template>
    </ContentBlock>

    <StatsBlock>
      The total amount of residential <br />
      transations has increasd by 22% <br />
      over the last year in Toronto.
    </StatsBlock>

    <ContentBlock background="#314259" color="#fff" sectionName="s-Leasing">
      <template #title>
        <h2>Leasing</h2>
      </template>
      <template #content>
        <p>
          Let us help you navigate through the neighborhoods of Toronto and the
          growing demand of the housing market in Toronto.
        </p>
        <div class="p-Home_ButtonsWrap">
          <button class="g-Button">
            what is the average rental price is in Toronto?
          </button>
        </div>
      </template>
      <template #svg>
        <LeasingSVG />
      </template>
    </ContentBlock>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue';
import Hero from '~/components/Hero.vue';
import StatsBlock from '~/components/StatsBlock.vue';
import ContentBlock from '@/components/ContentBlock.vue';
import BuyingSVG from '@/components/svg/Buying.vue';
import SellingSVG from '@/components/svg/Selling.vue';
import LeasingSVG from '@/components/svg/Leasing.vue';

export default {
  components: {
    Logo,
    Hero,
    StatsBlock,
    ContentBlock,
    BuyingSVG,
    SellingSVG,
    LeasingSVG
  }
};
</script>

<style lang="scss">
.p-Home_ButtonsWrap {
  margin-top: 35px;

  .g-Button {
    display: block;
    margin-bottom: 15px;
  }
}
.c-ContentBlock.s-Buying {
  padding-bottom: 20vh;
}
.c-ContentBlock.s-Selling {
  padding-bottom: 20vh;
}
.c-ContentBlock.s-Leasing {
  padding-bottom: 20vh;
}
</style>
