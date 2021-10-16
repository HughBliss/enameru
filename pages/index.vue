<template>
  <div class="main-page">
    <hero />
    <gallery />
    <features />
    <e-quote />
    <about />
  </div>
</template>

<script>
import Hero from '~/components/hero'
import Gallery from '~/components/gallery'
import Features from '~/components/features'
import EQuote from '~/components/e-quote'
import About from '~/components/about'

export default {
  components: {
    About,
    EQuote,
    Features,
    Gallery,
    Hero
  }
}
</script>
