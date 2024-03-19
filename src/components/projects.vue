<template>
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
</template>

<script>
export default {
  name: "main-projects",
  data() {
    return {
      project: [
        {
          project_id: '1',
          project_name: 'project name 1th',
          project_description: 'project description',
          project_image: 'project image',
          project_link: 'project link 1th'
        },
        {
          project_id: '2',
          project_name: 'project name 2th',
          project_description: 'project description',
          project_image: 'project image',
          project_link: 'project link 2th'
        },
        {
          project_id: '3',
          project_name: 'project name 3th',
          project_description: 'project description',
          project_image: 'project image',
          project_link: 'project link 3th'
        },
      ]
    }
  }
}
</script>

<style scoped>

</style>