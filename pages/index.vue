<template>
  <div class="main-page">
    <hero />
    <gallery></gallery>
  </div>
</template>

<script>
import Hero from '~/components/hero'
import Gallery from '~/components/gallery'

export default {
  components: {
    Gallery,
    Hero
  }
}
</script>
