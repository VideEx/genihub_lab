<template>
<!--  <div>-->
<!--    <label for="select">-->
<!--      Выберите тип работ:-->
<!--    </label>-->
<!--  </div>-->
  <select id="select">
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
select {
  width: 357px;
  padding: 25px;

  /*border: none;*/
  border: 10px solid;
  border-image-slice: 1;
  border-width: 3px;
  border-top: 0;
  border-right: 0;
  border-left: 0;
  /*border-bottom: 3px solid green;*/
  border-image-source: linear-gradient(135deg, rgba(193, 99, 166, 0.5), rgba(10, 49, 130, 0.5));

  font-size: 18px;

  background: transparent;

  margin-bottom: 25px;
}

select:focus {
  outline: none;
}

</style>
