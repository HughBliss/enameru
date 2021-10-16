<template>
  <section class="features section">
    <div class="container">
      <div class="features__wrap">
        <h2 class="section__title">
          Почему именно мы
        </h2>
        <p class="section__description">
          Мы сконцентрированы на главных ценностях и нуждах наших клиентов
        </p>
        <div class="features__grid">
          <div v-for="(f, key) in features" :key="key" class="features__item feature">
            <div class="feature__icon">
              <img :src="f.img" alt="">
            </div>
            <h3 class="feature__title">
              {{ f.title }}
            </h3>
            <p class="feature__description">
              {{ f.desc }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Features',
  data: () => ({
    features: [
      {
        img: require('~/assets/images/icons/star.svg'),
        title: 'Высокое качество',
        desc: 'Многолетний опыт работы дает возможность браться за проекты любой сложности.'
      },
      {
        img: require('~/assets/images/icons/operator.svg'),
        title: 'Индивидуальный подход',
        desc: 'Каждый клиент уникален. Мы разрабатываем уникальные концепции для каждого.'
      },
      {
        img: require('~/assets/images/icons/documents.svg'),
        title: 'Гарантии',
        desc: 'Со всеми клиентами мы работаем только официально и даем гарантии на все виды работ.'
      },
      {
        img: require('~/assets/images/icons/worker.svg'),
        title: 'Профессионалы',
        desc: 'Все члены нашей команды имеют большой опыт в работе, разработке и дизайне.'
      },
      {
        img: require('~/assets/images/icons/crown.png'),
        title: 'Поразительные возможности',
        desc: 'Прямая адгезия ко многим материалам, наличие специальных грунтов и добавок.'
      },
      {
        img: require('~/assets/images/icons/ticket.png'),
        title: 'Эксклюзивность',
        desc: 'Покраской можно впечатлить любого. А покрасить можно всё, что угодно.'
      }
    ]
  })
}
</script>

<style scoped>

</style>
