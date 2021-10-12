<template>
  <div class="pa-3">
    <h1>Sobre</h1>
      <p>
        Essa é uma lista de tarefas desenvolvida com Vue.js. 
      </p>
       
      <p>
        Algumas ferramentas utilizadas aqui foram:
      </p>
      <v-list>
      <template v-for="(item) in tacnologias">

        <v-list-item
          :key="item.titulo"
        >
          <v-list-item-avatar>
            <v-icon>{{item.icon}}</v-icon>
          </v-list-item-avatar>

          <v-list-item-content>
            <v-list-item-title v-html="item.titulo"></v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </template>
    </v-list>
    <hr>
    <section>
      <p>
        <v-card-subtitle >Contato:</v-card-subtitle>
        <v-card-text>
        <strong>📨E-mail:</strong>walisson_souza7@hotmail.com<br>
        <strong>🧑‍💻 Walisson Souza</strong><br>
        <img src="../assets/octocat.png" height="20px" alt="imagem octocat" /> <a href="https://github.com/walisson27">/WalissonSouza</a>
        </v-card-text>
      </p>
    </section>
      
  </div>
</template>

<script>

export default {
  data() {
    return{
      tacnologias:[
        {
          titulo: "HTML",
          icon: "mdi-language-html5"
        },
        {
          titulo: "Vue.js",
          icon: "mdi-vuejs"
        },
        {
          titulo: "Vuetify",
          icon: "mdi-vuetify"
        },
        {
          titulo: "VUEX",
          icon: "mdi-vuejs"
        },
        {
          titulo: "VueRouter",
          icon: "mdi-vuejs"
        },
        {
          titulo: "Localbase DB",
          icon: "mdi-database"
        },
        {
          titulo: "Animate.css",
          icon: "mdi-transition"
        },
        {
          titulo: "Drag and Drop",
          icon: "mdi-drag-variant"
        },
        {
          titulo: "Git",
          icon: "mdi-git"
        },
        {
          titulo: "GitHub",
          icon: "mdi-github"
        },
      ]
    }
  }
}
</script>

