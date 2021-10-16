<template>
  <div class="main-page">
    <hero />
    <gallery />
    <features />
  </div>
</template>

<script>
import Hero from '~/components/hero'
import Gallery from '~/components/gallery'
import Features from '~/components/features'

export default {
  components: {
    Features,
    Gallery,
    Hero
  }
}
</script>
