<template>
      <input type="text">
</template>

<script>
export default {
  name: "formInput"
}
</script>

<style scoped>
  input[type='text'] {
    width: 303px;
    padding: 25px;

    margin-bottom: 25px;

    border: none;

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
  }

  input[type='text']:focus {
    outline: none;
  }
</style>