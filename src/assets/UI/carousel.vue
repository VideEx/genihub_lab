<template>
  <div class="container">
    <h2 class="title linear">
      Команда
    </h2>
    <Carousel class="carousel" :items-to-show="1" :wrap-around="true">
      <Slide v-for="slide in team" :key="slide">
        <div class="carousel__item">
          <div class="carousel__item-stack">
            <ol>
              <li class="stack" v-for="item in slide.stack" :key="item">
                {{ item }}
              </li>
            </ol>
          </div>
          <div class="participant">
            {{ slide.participant }}
          </div>
        </div>
      </Slide>

      <template #addons>
        <!--      <Navigation />-->
        <Pagination/>
      </template>
    </Carousel>
  </div>
</template>

<script>
// import {callWithAsyncErrorHandling, defineComponent} from 'vue'
import {Carousel, Slide, Pagination} from 'vue3-carousel'
// import { Carousel, Navigation, Slide, Pagination } from 'vue3-carousel'

import 'vue3-carousel/dist/carousel.css'

export default {
  name: 'WrapAround',
  // methods: {callWithAsyncErrorHandling},
  components: {
    Carousel,
    Slide,
    // Navigation,
    Pagination
  },
  data() {
    return {
      team: [
        {
          id: 1,
          participant: 'Злакоманова Ксения',
          stack: {
            1: 'Системный анализ',
            2: 'JavaScript',
            3: 'VueJS',
            4: 'TS',
            5: 'HTML, CSS, JS',
          }
        },
        {
          id: 2,
          participant: 'Шебарин Саввелий',
          stack: {
            1: 'Java',
            2: 'Spring',
            3: 'Kotlin'
          }
        },
        {
          id: 3,
          participant: 'Якутина Дарья',
          stack: {
            1: 'Adobe Photoshop',
            2: 'Adobe Illustrator',
            3: 'Figma',
            4: 'Adobe After Effects',
            5: 'Blender 3D',
            6: 'Tilda'
          }
        },
        {
          id: 4,
          participant: 'Жуков Алексей',
          stack: {
            1: 'HTML CSS, SCSS, JS, TS',
            2: 'jQuery, bootstrap',
            3: 'React',
            4: 'React-redux',
            5: 'React-toolkit',
            6: 'Backend: Node.js, Express.js'
          }
        },
        {
          id: 4,
          participant: 'Соболь Сергей',
          stack: {
            1: 'Asp.Net Core',
            2: 'typescript',
            3: 'React',
            4: 'docker',
            5: 'portainer, html, css, scss',
            6: 'python/Django',
            7: 'sqlServer, PostgreSql'
          }
        }
      ]
    }
  }
}
</script>

<style>
.carousel {
  padding-top: 155px;
  padding-bottom: 20px;
  /*width: 700px;*/
}

.carousel__item {
  background: white;
  width: 700px;
  box-shadow: -4px 4px 4px rgba(0, 0, 0, 0.25);

  border-radius: 8px;

  margin-bottom: 20px;
}

.participant {
  background-image: linear-gradient(135deg, rgba(193, 99, 166, 0.5), rgba(10, 49, 130, 0.5));
  border-bottom-left-radius: 8px;
  border-bottom-right-radius: 8px;
  font-size: 30px;

  padding: 20px 0;

  color: white;
}

.stack {
  text-align: left;
}

.carousel__item-stack {
  padding: 15px 67px;

}
</style>