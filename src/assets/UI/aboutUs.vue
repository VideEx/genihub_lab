<template>
  <div class="about-list">
    <div class="about-card" v-bind:key="item" v-for="item in cards">
{{ item.card_description }}
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
          card_description: 'Ведущие разработчики',
        },
        {
          card_id: 1,
          card_description: 'Ведущие разработчики',
        },
        {
          card_id: 1,
          card_description: 'Ведущие разработчики',
        },
        {
          card_id: 1,
          card_description: 'Ведущие разработчики',
        },

      ]
    }
  }
}
</script>

<style scoped>

</style>