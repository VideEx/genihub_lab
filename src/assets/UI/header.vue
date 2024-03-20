<template>
  <div class="container header">
    <nav class="menu">
      <div class="menu__link">
        <a v-for="link in links" :key="link" :href="link.href">
          {{ link.content }}
        </a>
      </div>
      <button class="btn menu__actions">
        Оставить заявку
      </button>
    </nav>
  </div>
</template>

<script>
export default {
  name: "main-header",
  data() {
    return {
      links: [
        {
          href: '#',
          content: 'О нас'
        },
        {
          href: '#',
          content: 'Команда'
        },
        {
          href: '#',
          content: 'Проекты'
        },
        {
          href: '#',
          content: 'Отзывы'
        },
      ]
    }
  }
}
</script>

<style scoped>


.menu__link {
  width: 470px;
  display: flex;
  justify-content: space-between;
}

.menu__link a {
  color: #363333;
  text-decoration: none;
}

.menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
}



</style>