<template>
  <Head><Title>Home | Micky Rat</Title></Head>
  <header class="min-h-screen lg:h-screen bg-secondary">
    <div class="lg:flex items-center gap-24 h-full max-w-7xl lg:w-[80vw] container mx-auto px-6 py-20 lg:py-0">
      <img src="@/assets/images/logo-nobg.svg" class="h-screen-70 aspect-auto mx-auto" alt="">
      <div>
        <h1 class="text-9xl honey hidden lg:block">Micky Rat</h1>
        <UiTypographyP class="w-full mt-4">Micky Rat is a unique meme/Utility Token that seeks to reward investors by ensuring profitable return on investment (ROI) through the building and development of service utilities, powered by the Micky Rat tokens and distribute 30% of annual profits to investors in BNB or pay back profits into the liquidity Pool in order to keep the token price afloat to the benefit of all investors. Micky Rat also seeks to create value and serve as a reward token for exceptional performers in various fields of operations by the use of the Micky Rat Swap and NFTs Marketplace. This project is engineered and developed by a team of smart contract and DAPP developers with the name Micky Rat.  Micky Rat Foundation promises a fun and interactive engagement throughout its stay in the Crypto space. It aims to support children in need across Africa and Asia aside its load of investor-profitable utilities.</UiTypographyP>

        <div class="flex gap-8 mt-8">
        <NuxtLink to="https://t.me/Mickyratbsc" class="group py-2 px-5 text-black focus:text-white hover:text-white bg-secondary hover:bg-primary focus:outline-primary border-primary border font-medium text-base 2xl:text-lg justify-center duration-300 ease-in-out rounded-md outline-none focus:outline-none flex items-center gap-4">
          <IconsTelegram class="w-7 h-7 text-black group-hover:text-white duration-300 ease-in-out" />
          <UiTypographyP>Join Telegram</UiTypographyP> 
        </NuxtLink>
        <NuxtLink to="https://t.me/Mickyratbsc" class="group py-2 px-5 text-black focus:text-white hover:text-white bg-secondary hover:bg-primary focus:outline-primary border-primary border font-medium text-base 2xl:text-lg justify-center duration-300 ease-in-out rounded-md outline-none focus:outline-none flex items-center gap-4">
          <IconsTwitter to="https://twitter.com/rat_micky55647" class="w-7 h-7 text-black group-hover:text-white duration-300 ease-in-out" />
          <UiTypographyP>Follow on Twitter</UiTypographyP> 
        </NuxtLink>

        </div>
      </div>
    </div>

  </header>

  <section class="max-w-7xl py-20 px-6 container mx-auto">
    <ul class="grid lg:grid-cols-3 gap-16">
      <Cards v-for="item in items" :key="item.id">
        <UiTypographyH1 class="text-primary">{{item.title}}</UiTypographyH1>
        <UiTypographyP class="mt-8">{{ item.description }}</UiTypographyP>
      </Cards>
    </ul>
  </section>

  <section class="bg-secondary">
    <div class="animated py-20 px-6 ">
      <div class="grid lg:grid-cols-2 gap-12 max-w-7xl container mx-auto">
        <div class="rounded-3xl border border-primary p-8">
          <UiTypographyH1>Mission Statement</UiTypographyH1>
          <UiTypographyP class="mt-6">Micky Rat project is to simply reward exceptionalism and to be a prestigious mark of excellence and honour for top performers in the world. Micky Rat also is of the view that cryptocurrency holders and investors must be able to gain sustainable return on investment (ROI) whiles purchasing or holding coins and tokens of various projects that they trusted and believed in. In view of this and as a group of experienced application developers, we aim to create various utilities that would bring substantial returns to the investor by creating value for Micky Rat token and also making yearly distribution of partial profits realised from our utility applications, with all holders and investors of our project.</UiTypographyP>
        </div>
        <div class="rounded-3xl border border-primary p-8">
          <UiTypographyH1>Vision Statement</UiTypographyH1>
          <UiTypographyP class="mt-6">Micky Rat project is to simply reward exceptionalism and to be a prestigious mark of excellence and honour for top performers in the world. Micky Rat also is of the view that cryptocurrency holders and investors must be able to gain sustainable return on investment (ROI) whiles purchasing or holding coins and tokens of various projects that they trusted and believed in. In view of this and as a group of experienced application developers, we aim to create various utilities that would bring substantial returns to the investor by creating value for Micky Rat token and also making yearly distribution of partial profits realised from our utility applications, with all holders and investors of our project.</UiTypographyP>
        </div>
      </div>

    </div>
  </section>

  <section id="tokenomics" class="max-w-7xl py-20 px-6 container mx-auto text-center">
    <UiTypographyH1 class="text-primary">Tokenomics</UiTypographyH1>
    <UiTypographyP>Name: Micky Rat<br/>Symbol: Micky<br/>Decimal: 9<br/>Total supply: 1,000,000,000 <br/><br/>Tax 8%<br/>Marketing 4%
    <br/>Liquidity pool 1%<br/>Reflection 3%</UiTypographyP>
  </section>

  <section id="roadmap" class="max-w-7xl py-20 px-6 container mx-auto">
    <UiTypographyH1 class="text-primary text-center">Road Map</UiTypographyH1>
    <ul class="grid md:grid-cols-2 xl:grid-cols-4 gap-12 mt-8">
      <Cards>
        <UiTypographyH1 class="text-primary">Phase 1</UiTypographyH1>
        <UiTypographyP>Token creation and deployment.<br/>Project awareness marketing.<br/>Fair launch.<br/>Website.<br/>White paper.</UiTypographyP>
      </Cards>
      <Cards>
        <UiTypographyH1 class="text-primary">Phase 2</UiTypographyH1>
        <UiTypographyP>Token rollout on DEX.<br/>Marketing/Partnership with YouTube and other crypto influencers to create awareness.<br/>CMC Listing.<br/>CG Listing.</UiTypographyP>
      </Cards>
      <Cards>
        <UiTypographyH1 class="text-primary">Phase 3</UiTypographyH1>
        <UiTypographyP>Staking pool.<br/>Finalizing the development of the MICKYRATSWAP Platform.<br/>Making live the MICKYRATSWAP Platform.</UiTypographyP>
      </Cards>
      <Cards>
        <UiTypographyH1 class="text-primary">Phase 4</UiTypographyH1>
        <UiTypographyP>NFTs Marketplace.'<br/>CEX Listing Applications & Possible CEX Listing if approved.</UiTypographyP>
      </Cards>
    </ul>
  </section>
</template>
<script>
export default {
  data() {
    return {
      items: [
        {
          id: 1,
          title: 'Micky Rat Swap',
          description: `MickyRatSwap,is a decentralized exchange which would be deployed in the very early stages of the project. It is in the final stages of development and would provide passive income to all investors by distributing 30% of the yearly profit to all holders in a ratio of how much Micky Rat tokens they hold in BNB or send it in to the liquidity pool to help increase the overall price of the token as would be decided by the community.`,
        },
        {
          id: 2,
          title: 'NFTs Marketplace',
          description: `One of the most exciting avenues that Micky Rat aims to explore is the integration of Non-Fungible Tokens (NFTs). Recognizing the transformative potential of NFTs in establishing digital ownership and enabling new types of online commerce, Micky Rat will allow users to trade and auction NFTs alongside traditional goods in their NFTs Marketplace. This integration is not merely an addition but a significant part of our long-term strategy to remain at the forefront of blockchain-based commerce innovations.`,
        },
        {
          id: 3,
          title: 'Trading Bot',
          description: `Micky Rat will be building a trading bot that will make it's investors to trade other cryptocurrency easily and faster using Micky Rat trading bot.`,
        },
      ],
    }
  },
}
</script>
<style>
.animated {
  background-image: url('@/assets/images/bg.svg');
  background-size: cover;
  background-repeat: no-repeat;
}
</style>