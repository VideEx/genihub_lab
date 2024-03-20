<template>
  <footer>

    <div class="container footer">
      <div class="contacts">
        <p v-for="item in contacts" :key="item">
          {{ item.content }}
        </p>
      </div>
      <div class="info">
        <p>
          Разработано <span>Genihub Lab</span>
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "mainFooter",
  data() {
    return {
      contacts: [
        {
          content: '+79957930192'
        },
        {
          content: 'zlakomanovakv@gmail.com'
        }
      ]
    }
  }
}
</script>

<style scoped>
span {

}

footer  {
  color: white;
  background-image:  linear-gradient(135deg, rgba(193, 99, 166, 0.5), rgba(10, 49, 130, 0.5));
}

.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;

}
</style>