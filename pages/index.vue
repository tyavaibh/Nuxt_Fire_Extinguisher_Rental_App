<template>
  <div>
    <div>
      <Hero />

      <LargeCardDisplay
        v-for="cardInfo in largeCardInfo"
        :key="cardInfo.id"
        :cardsSection="cardInfo"
      />
      <SmallCardDisplay
        v-for="cardInfo in smallCardInfo"
        :key="cardInfo.id"
        :cardsSection="cardInfo"
      />
    </div>
  </div>
</template>

<script>
import { largeCardSections, smallCardSections } from '~/assets/data.js'

export default {
  name: 'IndexPage',

  data() {
    return {
      largeCardInfo: largeCardSections,

      smallCardInfo: smallCardSections,
    }
  },
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
</style>
