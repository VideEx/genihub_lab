<template>
  <div class="container">
    <div class="input" :key="item" v-for="item in inputData">
      <form-input v-bind:id="item.input_id"
                  :placeholder="item.input_placeholder" v-model="item.input_placeholder"></form-input>
    </div>
    <form-select></form-select>
    <form-submit></form-submit>
  </div>
</template>

<script>
import formSelect from "@/assets/UI/form_components/select.vue";
import formInput from "@/assets/UI/form_components/input.vue";
import formSubmit from "@/assets/UI/form_components/submit.vue";

export default {
  name: "mainOrder",
  components: {
    formSelect,
    formInput,
    formSubmit
  },
  data() {
    return {
      inputData: [
        {
          input_id: 'user_name',
          input_placeholder: 'Ваше имя',
          input_name: 'userName'
        },
        {
          input_id: 'user_phone',
          input_placeholder: 'Ваш номер телефона',
          input_name: 'userPhone'
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>