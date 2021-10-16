<template>
  <div>
    <div v-show="isMenuOpen" class="header__menu-screen"/>
    <div class="header">
      <div class="container">
        <nav class="header__nav">
          <button
            :class="{'header__menu-button--opened': isMenuOpen}"
            class="header__menu-button"
            @click="toggleMenu"
          >
            <span/>
          </button>
          <ul class="header__list header__list--one" :class="{'header__list--open': isMenuOpen}">
            <li class="header__list-item">
              <nuxt-link to="#" @click="toggleMenu">
                О нас
              </nuxt-link>
            </li>
            <li class="header__list-item">
              <nuxt-link to="#" @click="toggleMenu">
                Завод
              </nuxt-link>
            </li>
            <li class="header__list-item">
              <nuxt-link to="#" @click="toggleMenu">
                Преимущества
              </nuxt-link>
            </li>
          </ul>
          <nuxt-link class="header__logo" to="/">
            <img alt="" class="" src="~assets/images/logo.jpg">
          </nuxt-link>
          <ul class="header__list header__list--two" :class="{'header__list--open': isMenuOpen}">
            <li class="header__list-item">
              <nuxt-link to="#" @click="toggleMenu">
                Заказать
              </nuxt-link>
            </li>
            <li class="header__list-item">
              <nuxt-link to="#" @click="toggleMenu">
                Контакты
              </nuxt-link>
            </li>
            <li class="header__list-item">
              <nuxt-link to="#" @click="toggleMenu">
                Наши работы
              </nuxt-link>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'EHeader',
  data: () => ({
    isMenuOpen: false
  }),
  methods: {
    toggleMenu () {
      this.isMenuOpen = !this.isMenuOpen
    }
  }
}
</script>

<style scoped>

</style>
