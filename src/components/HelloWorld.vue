<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <i class="fas large fa-code" id='fontColor'></i>
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3" id='fontColor'>
          Joshua Sayah
        </h1>

        <p class="subheading font-weight-regular" id='fontColor'>
          Welcome to my portfolio,<br>
          I am a software developer who loves learning new skills.<br>
          If you don't find the specific language you are looking for here dont worry!<br>
          Learning a new language is a breeze.
        </p>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
        id='background'
        style='border-radius: 5px;'
      >
        <h1 class="font-weight-bold mb-3">
          Projects
        </h1>

        <v-row justify="center">
          
          <a
            v-for="(project, i) in projects"
            :key="i"
            class="subheading mx-3"
            target="_blank"
            id='total'
          >
            <v-card id='card'>
              <h1>{{ project.title }}</h1><br>
              {{project.desc}}<br>
              <div id='links'><a :href="project.git" target="_blank" id='decoration'><i class="fab iconMain fa-github"></i><br>GitHub</a></div>
              <div id='links'><a :href="project.demo" target="_blank" id='decoration'><i class="fas iconMain fa-laptop-code"></i><br>Demo</a></div>
            </v-card>
          </a>
          
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'Home',

    data: () => ({
      projects: [
        {
          title: 'Virtual Terminal',
          git: 'https://vuetifyjs.com/components/api-explorer',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Massa vitae tortor condimentum lacinia quis vel. Vitae tortor condimentum lacinia quis vel eros donec. Lacus luctus accumsan tortor posuere ac. Sagittis purus sit amet volutpat consequat mauris nunc congue. Dictum sit amet justo donec enim diam. Et malesuada fames ac turpis egestas integer eget aliquet nibh. Massa ultricies mi quis hendrerit dolor magna eget. In nibh mauris cursus mattis molestie a iaculis at erat. Faucibus scelerisque eleifend donec pretium. Massa tempor nec feugiat nisl pretium fusce id velit. Elementum integer enim neque volutpat ac. At lectus urna duis convallis convallis tellus id interdum velit. Pharetra massa massa ultricies mi quis hendrerit dolor. Egestas pretium aenean pharetra magna ac placerat vestibulum lectus. Sit amet mattis vulputate enim nulla aliquet porttitor lacus luctus.',
          demo: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          title: 'Info API',
          git: 'https://vuetifyjs.com/getting-started/pre-made-layouts',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Massa vitae tortor condimentum lacinia quis vel. Vitae tortor condimentum lacinia quis vel eros donec. Lacus luctus accumsan tortor posuere ac. Sagittis purus sit amet volutpat consequat mauris nunc congue. Dictum sit amet justo donec enim diam. Et malesuada fames ac turpis egestas integer eget aliquet nibh. Massa ultricies mi quis hendrerit dolor magna eget. In nibh mauris cursus mattis molestie a iaculis at erat. Faucibus scelerisque eleifend donec pretium. Massa tempor nec feugiat nisl pretium fusce id velit. Elementum integer enim neque volutpat ac. At lectus urna duis convallis convallis tellus id interdum velit. Pharetra massa massa ultricies mi quis hendrerit dolor. Egestas pretium aenean pharetra magna ac placerat vestibulum lectus. Sit amet mattis vulputate enim nulla aliquet porttitor lacus luctus.',
          demo: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          title: 'Front End to Existing API',
          git: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Massa vitae tortor condimentum lacinia quis vel. Vitae tortor condimentum lacinia quis vel eros donec. Lacus luctus accumsan tortor posuere ac. Sagittis purus sit amet volutpat consequat mauris nunc congue. Dictum sit amet justo donec enim diam. Et malesuada fames ac turpis egestas integer eget aliquet nibh. Massa ultricies mi quis hendrerit dolor magna eget. In nibh mauris cursus mattis molestie a iaculis at erat. Faucibus scelerisque eleifend donec pretium. Massa tempor nec feugiat nisl pretium fusce id velit. Elementum integer enim neque volutpat ac. At lectus urna duis convallis convallis tellus id interdum velit. Pharetra massa massa ultricies mi quis hendrerit dolor. Egestas pretium aenean pharetra magna ac placerat vestibulum lectus. Sit amet mattis vulputate enim nulla aliquet porttitor lacus luctus.',
          demo: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          title: 'Admin Dashboard',
          git: 'https://vuetifyjs.com/components/api-explorer',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Massa vitae tortor condimentum lacinia quis vel. Vitae tortor condimentum lacinia quis vel eros donec. Lacus luctus accumsan tortor posuere ac. Sagittis purus sit amet volutpat consequat mauris nunc congue. Dictum sit amet justo donec enim diam. Et malesuada fames ac turpis egestas integer eget aliquet nibh. Massa ultricies mi quis hendrerit dolor magna eget. In nibh mauris cursus mattis molestie a iaculis at erat. Faucibus scelerisque eleifend donec pretium. Massa tempor nec feugiat nisl pretium fusce id velit. Elementum integer enim neque volutpat ac. At lectus urna duis convallis convallis tellus id interdum velit. Pharetra massa massa ultricies mi quis hendrerit dolor. Egestas pretium aenean pharetra magna ac placerat vestibulum lectus. Sit amet mattis vulputate enim nulla aliquet porttitor lacus luctus.',
          demo: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          title: 'Menu Manager',
          git: 'https://vuetifyjs.com/components/api-explorer',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Massa vitae tortor condimentum lacinia quis vel. Vitae tortor condimentum lacinia quis vel eros donec. Lacus luctus accumsan tortor posuere ac. Sagittis purus sit amet volutpat consequat mauris nunc congue. Dictum sit amet justo donec enim diam. Et malesuada fames ac turpis egestas integer eget aliquet nibh. Massa ultricies mi quis hendrerit dolor magna eget. In nibh mauris cursus mattis molestie a iaculis at erat. Faucibus scelerisque eleifend donec pretium. Massa tempor nec feugiat nisl pretium fusce id velit. Elementum integer enim neque volutpat ac. At lectus urna duis convallis convallis tellus id interdum velit. Pharetra massa massa ultricies mi quis hendrerit dolor. Egestas pretium aenean pharetra magna ac placerat vestibulum lectus. Sit amet mattis vulputate enim nulla aliquet porttitor lacus luctus.',
          demo: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          title: 'One Student Body',
          git: 'https://github.com/JSayah/osb',
          desc: 'This is my ongoing personal project. I hope someday for it to be a fully functional learning tool where people, no matter location or financial situation, can go to receive a quality education. I hope to achieve full accreditation and make a quality education available to anyone that wants one.',
          demo: 'https://github.com/JSayah/osb',
        },
      ],
    }),
  }
</script>
<style>
.large{
  font-size: 700%;
}
#background{
  background: linear-gradient(90deg, rgba(142,0,137,1) 0%, rgba(119,9,121,1) 35%, rgba(0,212,255,1) 100%);
}
#links{
  display:inline-block;
  vertical-align: top;
  padding: 20px;
  margin-top:10px;
}
#card{
  padding: 20px;
  margin: 20px;
  max-width: 800px;
}
.iconMain{
  font-size: 200%;
}
#decoration, #decoration:visited, #decoration:active {
  color: black;
  text-decoration: none;
}
#decoration:hover{
  color: orange;
}
#fontColor{
  color: white;
}
</style>