<template>
  <div class="main-page">
    <hero />
    <gallery />
    <features />
    <e-quote />
    <about />
    <advantages />
    <callback />
    <contacts />
  </div>
</template>

<script>
import Hero from '~/components/hero'
import Gallery from '~/components/gallery'
import Features from '~/components/features'
import EQuote from '~/components/e-quote'
import About from '~/components/about'
import Advantages from '~/components/advantages'
import Callback from '~/components/callback'
import Contacts from '~/components/contacts'

export default {
  components: {
    Contacts,
    Callback,
    Advantages,
    About,
    EQuote,
    Features,
    Gallery,
    Hero
  }
}
</script>
