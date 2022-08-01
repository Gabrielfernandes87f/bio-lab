<template>
  <div class="index-desktop">
    <div>
      <div class="theme" :id="desktopTheme">
        <span @click="darkMode" class="material-icons"> bedtime </span>
      </div>
      <div class="div-img div-avatar">
        <img
          class="avatar-perfil"
          src="@/assets/img/perfil.jpg"
          alt="avatar"
          srcset="@/assets/img/perfil.jpg"
        />
      </div>
      <div>
        <div class="description-body">
          <div class="div-flex-center">
            <h1 class="name">Gabriel Fernandes</h1>
          </div>
          <div class="div-flex-center">
            <h2>Desenvolvedor Fullstack</h2>
          </div>
          <div class="div-flex-center">
            <h3>PHP - Laravel - VueJs - NuxtJs - SQL</h3>
          </div>
          <hr />
          <div class="description-desktop">
            <p class="flex-center">
              Resolvendo problemas digitais de empresários ou instiuições no que
              tange a propagações das informações sobre seus negócios e suas
              atividades. visando a captação de novos clientes e aumentando os
              lucros, ao mesmo tempo que ajuda a melhorar a qualidade de vida
              dos seus usuários.
            </p>
          </div>
        </div>
      </div>
      <div class="div-flex-center email-desktop">Gabriel1coder@gmail.com</div>

      <div>
        <a
          href="https://github.com/Gabrielfernandes87f"
          target="_blank"
          class=""
        >
          <div class="card">
            <span class="material-icons"> label_important </span>
            <p>Github</p>
            <span class="material-icons"> label_important </span>
          </div>
        </a>
      </div>
      <div>
        <a
          href="https://www.linkedin.com/in/gabrielfernandesweb/"
          target="_blank"
        >
          <div class="card">
            <span class="material-icons"> label_important </span>
            <p>LinkedIn</p>
            <span class="material-icons"> label_important </span>
          </div>
        </a>
      </div>
      <div>
        <nuxt-link to="projetos" target="_blank">
          <div class="card">
            <span class="material-icons"> label_important </span>
            <p>Projetos</p>
            <span class="material-icons"> label_important </span>
          </div>
        </nuxt-link>
      </div>
      <div>
        <a
          href="https://www.instagram.com/gabriel.fernandes.f/"
          target="_blank"
        >
          <div class="card">
            <span class="material-icons"> label_important </span>
            <p>Instagram</p>
            <span class="material-icons"> label_important </span>
          </div>
        </a>
      </div>
      <div>
        <a href="https://github.com/Gabrielfernandes87f" target="_blank">
          <div class="card">
            <span class="material-icons"> label_important </span>
            <p>Whatsapp</p>
            <span class="material-icons"> label_important </span>
          </div>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home-web",
  data() {
    return {
      dark: false,
      light: true,
      desktopTheme: "",
    };
  },
  methods: {
    darkMode() {
      this.light = !this.light;
      this.dark = !this.dark;
      console.log(this.light);
    },
  },
  mounted() {
    if (localStorage.getItem("darkMode") == "true") {
      this.dark = true;
      this.desktopTheme = "light";
      this.light = false;
    } else {
      this.desktopTheme = "dark";
      this.dark = false;
      this.light = true;
    }
  },
  watch: {
    dark: function (newVal, oldVal) {
      if (newVal) {
        localStorage.setItem("darkMode", "true");
        document.body.classList.add("darkMode");
        this.desktopTheme = "light";
      } else {
        localStorage.setItem("darkMode", "false");
        this.desktopTheme = "dark";
      }
    },
    light: function (newVal, oldVal) {
      if (newVal) {
        localStorage.setItem("darkMode", "false");
        document.body.classList.remove("darkMode");
      } else {
        localStorage.setItem("darkMode", "true");
        document.body.classList.add("darkMode");
        document.body.classList.remove("darkMode-off");
      }
      console.log(localStorage.darkMode + "test");
    },
  },
};
</script>
