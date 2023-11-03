<template>
  <Head><Title>Home | Santa Inu</Title></Head>
  <header class="min-h-screen background text-white">
    <div class="gap-24 max-w-7xl mx-auto px-6 pb-8">
      <main class="lg:w-1/2">
        <img src="/favicon.png" class="h-screen-70 aspect-auto mx-auto" alt="">
        <div>
          <UiTypographyH1>Santa Inu</UiTypographyH1>
          <UiTypographyP class="w-full mt-4">Christmas is around the corner! <br />The season of giving is here and the revolutionary meme token Santa Inu is planning to give back in huge amounts to holders leading up to Christmas. 💵70% taxes generated are use to buyback into Micky Rat. 20% taxes are converted into USDT and given to holders who purchase Santa inu and hold as a reflection rewards. 10% will be for marketing of Santa inu.<br />Santa inu is not just a festival memetoken  is a meme token operating on the BEP-20 Blockchain technology (Binance Smart Chain).Santa inu aims to be one of the most successful Christmas project in 2023 and the years to come, with 20% usdt rewards every day to its holders! We are taking advantage of the upcoming Holiday to gain the crypto community's attention but as the weeks go by, this project will gain its reputation through continuous communication with its investors, aggressive marketing campaigns, listings, and constant delivery from the leadership team. Kindly  invite your friends family love ones on this wonderful journey alongside our wonderful loyal community!</UiTypographyP>

          <div class="flex gap-8 mt-8">
          <NuxtLink to="https://t.me/santainu1only" class="group py-2 px-5 text-white focus:text-white hover:text-black bg-primary hover:bg-white focus:outline-primary font-medium text-base 2xl:text-lg justify-center duration-300 ease-in-out rounded-md outline-none focus:outline-none flex items-center gap-4">
            <IconsTelegram class="w-7 h-7 text-white group-hover:text-black duration-300 ease-in-out" />
            <UiTypographyP>Join Telegram</UiTypographyP> 
          </NuxtLink>
          <NuxtLink to="https://twitter.com/santainuch/" class="group py-2 px-5 text-black focus:text-white hover:text-white bg-white hover:bg-primary focus:outline-primary font-medium text-base 2xl:text-lg justify-center duration-300 ease-in-out rounded-md outline-none focus:outline-none flex items-center gap-4">
            <IconsTwitter class="w-7 h-7 text-black group-hover:text-white duration-300 ease-in-out" />
            <UiTypographyP>Follow on Twitter</UiTypographyP> 
          </NuxtLink>

          </div>
        </div>
      </main>

    </div>

  </header>

  <section class="max-w-7xl py-20 px-6 container mx-auto">
    <UiTypographyH2 class="text-center">What are out features?</UiTypographyH2>
    <ul class="grid lg:grid-cols-3 gap-16 mt-8">
      <Cards v-for="item in items" :key="item.id">
        <UiTypographyH2 class="text-primary">{{item.title}}</UiTypographyH2>
        <UiTypographyP class="mt-8">{{ item.description }}</UiTypographyP>
      </Cards>
    </ul>
  </section>

  <section id="tokenomics" class="md:flex gap-8 py-20 items-center">
    <img src="/image.jpg" alt="" class="md:w-1/2">

    <div class="md:w-1/2 mt-8 md:mt-0 px-6">
      <UiTypographyH1 class="text-primary">Tokenomics</UiTypographyH1>
      <UiTypographyP>Name: Santa inu<br/>Symbol: Santa<br/>Decimal: 18<br/>Total supply: 100,000,000 Santa<br/>5% Buy Tax - 9% Sell <br/><br /><span><UiTypographyH2>Tax:</UiTypographyH2></span>2% Rewards: Dividend tax on all transactions that will be distributed every 24 hours to holders in usdt.<br/>3% Marketing: Marketing tax on all transactions allows the Santa inu marketing team to reinvest and grow the project to its maximum potential.<br/>1% Liquidity: Liquidity tax on all transactions to prevent major price fluctuation after a large trade by filling the liquidity pool.<br />3% Micky Rat Buyback: buyback tax on all transactions allows the devs to buyback Micky Rat for the growth of the Micky Rat project. </UiTypographyP>
    </div>
  </section>
  <section id="roadmap" class="max-w-7xl py-20 px-6 container mx-auto">
    <UiTypographyH1 class="text-primary text-center">Road Map</UiTypographyH1>
    <div class="mx-auto w-fit">
      <div class="mt-8 flex flex-row xl:flex-col gap-12">
        <div class="grid relative place-items-center w-10 xl:h-10 xl:w-auto">
          <ul class="grid xl:grid-cols-4 gap-12 absolute w-full h-full place-items-center">
            <li v-for="phase in 4" >
              <div class="text-white font-bold h-10 w-10 bg-primary grid place-items-center mx-auto rounded-full">
                {{ phase }}
              </div>
            </li>
          </ul>
          <div class="xl:w-full bg-primary xl:h-1 h-full w-1 mx-auto"></div>
        </div>

        <ul class="grid xl:grid-cols-4 gap-12">
          <Cards>
            <UiTypographyH2 class="text-primary">Phase 1</UiTypographyH2>
            <UiTypographyP>Contract creation.<br/>Website development.<br/>Media Creation.<br/>Marketing.</UiTypographyP>
          </Cards>
          <Cards>
            <UiTypographyH2 class="text-primary">Phase 2</UiTypographyH2>
            <UiTypographyP>Marketing Campaign.<br/>Marketing Campaign.<br/>Launch on PancakeSwap.<br/>Dextool trending.<br/>AMA</UiTypographyP>
          </Cards>
          <Cards>
            <UiTypographyH2 class="text-primary">Phase 3</UiTypographyH2>
            <UiTypographyP>Partnership.<br/>Reward Tracker.<br/>Twitter space.<br/>Airdrop Partnership<br/>Farm & Staking Pools</UiTypographyP>
          </Cards>
          <Cards>
            <UiTypographyH2 class="text-primary">Phase 4</UiTypographyH2>
            <UiTypographyP>CMC/CG Listings.<br/>NFT Collection Launch.<br/>Influencers Campaign.<br/>Christmas Charity Donation.</UiTypographyP>
          </Cards>
        </ul>
      </div>
    </div>

  </section>
</template>
<script>
export default {
  data() {
    return {
      items: [
        {
          id: 1,
          title: '$USDT Rewards',
          description: `Earn automatic ($USDT), rewards by holding your SANTA INU- 2% of every buy, transfer and sell transaction is redistributed automatically to $SANTA INU holders. You will receive the rewards automatically in your wallet.`,
        },
        {
          id: 2,
          title: 'Marketing',
          description: `3% of every transaction will directly go to the marketing wallet in order to ensure an increase in exposure throughout advertisement platforms, social media and to secure contracts and deals with influencers. This will help Santa inu achieve an international status and to be known within every community!`,
        },
        {
          id: 3,
          title: 'Liquidity Pool',
          description: `Our Smart contract deposits 1% from every transaction as $santa inu and $BNB into a liquidity pool which has been locked and certified. Pancakeswap fixes the low liquidity problems of DEXs through their Liquidity Pools, ensuring traders can always Buy & Sell without liquidity issues. A bigger liquidity pool will provide more stability for Santa inu liquidity pool.`,
        },
      ],
    }
  },
}
</script>
<style>
.background {
  background-image: url('/hero.svg');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
</style>