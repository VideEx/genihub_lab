<template>
  <div>
    <label for="select">
      Выберите тип работ:
    </label>
  </div>
  <select id="select">
    <option disabled value="">Please select one</option>
    <option v-for="item in options" :key="item">
      {{ item.option_description }}
    </option>
  </select>
</template>

<script>

export default {
  name: "formSelect",
  data() {
    return {
      options: [
        {
          option_id: 1,
          option_description: 'Разработка сайта'
        },
        {
          option_id: 1,
          option_description: 'Разработка сайта на конструкторе'
        },
        {
          option_id: 1,
          option_description: 'Поддержка сайта'
        },
        {
          option_id: 1,
          option_description: 'СЕО оптимизация'
        },
        {
          option_id: 1,
          option_description: 'Разработка дизайн макета сайта'
        }
      ]
    }
  },
  methods: {
  }
}
</script>

<style scoped>

</style>
