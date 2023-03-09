<template lang="pug">
    v-main.grey.darken-4
      v-container
        v-layout.d-flex.column
          v-flex.d-flex.mb-6
            v-img(src='/photo.jpg').photo-size.mr-6
            h1.yellow--text.text--darken-3.text-h1.d-flex.align-center Сайт-портфолио<br> Хапилиной Альбины
          v-flex.d-flex.justify-center.mb-10
            v-btn.yellow.darken-3 Посмотреть резюме на HH.ru
          v-flex.mb-9
            v-layout.d-flex.column.justify-center.align-center.about__section.grey.darken-4.blue-grey--text.text--lighten-5.pa-6
              h2.blue-grey--text.text--lighten-5.mb-8 О себе
              p Меня зовут Альбина. Занимаюсь разработкой и дизайном с 2019 года.
              p Используемые технологии: HTML5, CSS3, JavaScript, git,  SCSS, JQuery, Bootstrap. Самостоятельно разрабатываю дизайн с помощью Figma, Adobe illustrator.
              p Опыт работы с Swiper JS, версткой email-писем.
              p Изучаю новые технологии во frontend-разработке, хочу расти и развиваться в данной сфере.
              p Более подробное резюме можете просмотреть
              a(href="").yellow--text.text--darken-3 на сайте hh.ru (ссылка)
          v-flex.mb-9
            v-layout.d-flex.column.justify-center.align-center.blue-grey--text.text--lighten-5
              h2.text-center.mb-8 Опыт работы
                v-expansion-panels(variant="accordion")
                  v-expansion-panel(v-for="i in 3" :key="i" title="Item" text="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.")

          v-flex.mb-9
            v-layout.d-flex.column.justify-center.align-center.blue-grey--text.text--lighten-5
              h2.mb-8 Работы в Adobe Illustrator
              v-sheet.mx-auto(dark max-width='1000')
                v-slide-group.grey.darken-4
                  v-slide-group-item(v-for="(slide, i) in slides" :key="i")
                    v-img(height="200px" max-width='300px' contain :src="slide.link")



          v-flex.blue-grey--text.text--lighten-5
              v-layout.d-flex.column.justify-center.align-center.blue-grey--text.text--lighten-5
                h2.mb-8 Контакты
                p Если вы хотите связаться со мной :
                p мой почтовый ящик
                a(href="").yellow--text.text--darken-3 albinabist1993@mail.ru
                p или
                p оставьте свою почту и выберите цель общения.





</template>

<!--  v-main-->
<!--    v-container-->
<!--      div-->
<!--        h1 Сайт-портфолио<br> Хапилиной Альбины-->
<!--        a(href="") Посмотреть резюме на HH.ru-->
<!--        section.about__section-->
<!--          h2 О себе-->
<!--          p Меня зовут Альбина. Занимаюсь разработкой и дизайном с 2019 года.-->
<!--          p Используемые технологии: HTML5, CSS3, JavaScript, git,  SCSS, JQuery, Bootstrap. Самостоятельно разрабатываю дизайн с помощью Figma, Adobe illustrator.-->
<!--          p Опыт работы с Swiper JS, версткой email-писем.-->
<!--          p Изучаю новые технологии во frontend-разработке, хочу расти и развиваться в данной сфере.-->
<!--          p Более подробное резюме можете просмотреть-->
<!--          a(href="") на сайте hh.ru (ссылка)-->

<!--        section.work-experience__section-->
<!--          div раскрывашка-->

<!--        section.my-works__section-->
<!--          div slider-->

<!--        section.contacts__section Контакты-->
<!--          p Если вы хотите связаться со мной :-->
<!--          p мой почтовый ящик-->
<!--          a(href="") albinabist1993@mail.ru-->
<!--          p или-->
<!--          p оставьте свою почту и выберите цель общения.-->




<script>
    export default {
        name: "app-main",
        data: () => ({
            drawer: null,
            model: null,
            slides: [
                {
                    alt: 'фото 1',
                    link: '/Albina.png',
                },
                {
                    alt: 'фото 2',
                    link: '/Mama.png',
                },
                {
                    alt: 'фото 3',
                    link: '/Boris.png',
                },
                {
                    alt: 'фото 4',
                    link: '/Is.png',
                },
                {
                    alt: 'фото 5',
                    link: '/Vika.png',
                },
                {
                    alt: 'фото 6',
                    link: '/Lera.png',
                }
                ]
        }),
        props: {
            source: String
        }
    }
</script>

<style>

  /*.main__section {*/
  /*  background: #141516;*/
  /*}*/

  .photo-size {
    max-width: 30%;
  }

  .about__section {
    box-shadow: 3px 3px 4px rgba(63, 65, 66, 0.3), -3px -3px 4px rgba(21, 22, 22, 0.5), inset -65px 65px 130px rgba(21, 22, 22, 0.2), inset 65px -65px 130px rgba(21, 22, 22, 0.2), inset -65px -65px 130px rgba(63, 65, 66, 0.9), inset 65px 65px 163px rgba(21, 22, 22, 0.9);
  }

  .v-slide-group__next, .v-slide-group__prev {
    background: transparent url("../static/arrow.svg") no-repeat center;
  }

  .v-slide-group__prev {
    transform: rotate(180deg);
  }

</style>
