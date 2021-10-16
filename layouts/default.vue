<template>
  <div class="layout">
    <e-header />
    <Nuxt />
  </div>
</template>
<script>
import EHeader from '~/components/layout/e-header'

export default {
  name: 'Default',
  components: { EHeader }
}
</script>

<style lang="scss">

</style>
