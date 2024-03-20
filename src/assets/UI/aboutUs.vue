<template>
  <div class="purple">
    <div class="container">
      <h2 class="title white">
        О нас
      </h2>
      <div class="about-list">
        <div class="about-card" v-bind:key="item" v-for="item in cards">
          {{ item.card_description }}
        </div>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: "aboutUs",
  data() {
    return {
      cards: [
        {
          card_id: 1,
          card_description: 'Практикующие разработчики, представители ведущих IT компаний.',
        },
        {
          card_id: 2,
          card_description: 'Обширный стек frontend и backend технологий',
        },
        {
          card_id: 1,
          card_description: 'Выполнение работ различной степени сложности. От лендингов и Wordpress сайтов до объемных web приложений',
        },
        {
          card_id: 1,
          card_description: 'Поможем грамотно сформулировать задачу и довести проект до идеала',
        },

      ]
    }
  }
}
</script>

<style scoped>
.about-list {
  display: flex;
  justify-content: flex-start;
  gap: 35px;
  flex-wrap: wrap;
}

.about-card {
  width: 494px;

  padding: 70px 34px;
  background: white;
  box-shadow: -4px 4px 4px rgba(0, 0, 0, 0.25);
  border-radius: 8px;

  z-index: 3;
}
</style>