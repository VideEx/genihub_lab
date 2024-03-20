<template>
  <div class="purple">
    <div class="container">
      <h2 class="title white">
        Проекты
      </h2>
      <div class="project_list">
        <div class="project_item" v-for="item in project" v-bind:key="item">
          <p>
            {{ item.project_name }}
          </p>
          <p>
            {{ item.project_link }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "main-projects",
  data() {
    return {
      project: [
        {
          project_id: '1',
          project_name: 'Лендинг детского лагеря',
          project_description: 'Лендинг детского лагеря',
          project_image: 'project image',
          project_link: 'https://camp.genihub.ru/'
        },
        {
          project_id: '2',
          project_name: 'Локальный квест к Дню Рождения',
          project_description: 'Локальный квест к Дню Рождения',
          project_image: 'project image',
          project_link: 'project link 2th'
        },
        {
          project_id: '3',
          project_name: 'Сайт образовательного центра ',
          project_description: 'Сайт образовательного центра ',
          project_image: 'project image',
          project_link: 'project link 3th'
        },
      ]
    }
  }
}
</script>

<style scoped>
.project_item {
  padding: 70px 50px;
  width: 428px;

  background: white;
  box-shadow: -4px 4px 4px rgba(0, 0, 0, 0.25);
  border-radius: 8px;
}

.project_list {
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-start;
  gap: 30px;
}

</style>