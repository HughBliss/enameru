<template>
  <section class="callback section">
    <div class="container">
      <h2 class="section__title">
        Оставить заявку на заказ:
      </h2>
      <p class="section__description">
        Укажите ваши контакты
      </p>
      <form
        class="callback__form"
        @submit.prevent="handleSubmit"
      >
        <input
          v-model="form.name"
          class="callback__input"
          placeholder="Имя"
          type="text"
        >
        <input
          v-model="form.email"
          class="callback__input"
          placeholder="Email"
          type="email"
        >
        <input
          v-model="form.phone"
          class="callback__input"
          placeholder="Телефон"
          type="text"
        >
        <button class="callback__submit" type="submit">
          Отправить заявку
        </button>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Callback',
  data: () => ({
    form: {
      name: '',
      email: '',
      phone: ''
    }
  }),
  methods: {
    handleSubmit () {
      console.log(this.form)
    }
  }
}
</script>

<style scoped>

</style>
