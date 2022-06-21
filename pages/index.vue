<template>
  <div class="index">
    <div class="body">
      <div class="desk-display">
        <h1>Bem vindos!</h1>
        <p>
          Fiz essa pagina apenas para divulgar o app
          <strong class="bio-lab">Bio-lab</strong>
        </p>
        <p>baixe na Play store</p>

        <a href="https://play.google.com/store/apps/details?id=com.app.tcc.tccapp" target="_blank">
          <img src="https://play.google.com/intl/en_us/badges/static/images/badges/pt-br_badge_web_generic.png"
            alt="Download Android" class="google-play" />
        </a>
        <p>Essa pagina foi otimizada pra dispositivos mobile.</p>
        <div class="div-flex-center">
          <p>Veja no seu computador</p>
          <a href="#" target="_blank" class="link-pc">clicando aqui </a>
        </div>
      </div>

      <div class="main">
        <div class="main-content">
          <div class="div-img div-avatar">
            <img class="avatar-perfil" src="@/assets/img/perfil.jpg" alt="avatar" srcset="@/assets/img/perfil.jpg" />
          </div>
          <div class="description-body">
            <div class="div-flex-center">
              <h1 class="name">{{ name }}</h1>
            </div>
            <div class="div-flex-center">
              <h2>{{ desccription }}</h2>
            </div>
            <div class="div-flex-center">
              <h3>{{ desccription2 }}</h3>
            </div>
            <hr />
            <p class="sub-title div-flex-center">{{ msg }}</p>
          </div>
        </div>
        <div class="content-description div-flex-center">
          <p>{{ contentText }}</p>
        </div>

        <div class="card meuslinks">
          <div class="div-flex-center">
            <h1>Gabriel1coder@gmail.com</h1>
          </div>
        </div>
        <!-- fim -->
        <div class="links-content-body">
          <div class="links-content card">
            <a href="https://github.com/Gabrielfernandes87f" target="_blank" class="nuxt-links">
              <div class="div-img img-content">
                <img class="img-svg" src="@/assets/img/github.png" alt="github" />
              </div>
              <span class="div-flex-center-end">Github</span>
            </a>
          </div>
        </div>
        <!-- fim -->
        <div class="links-content-body">
          <div class="links-content card">
            <a href="https://www.linkedin.com/in/gabrielfernandesweb/" target="_blank" class="nuxt-links">
              <div class="div-img img-content">
                <img src="@/assets/img/linkedin.png" alt="linkedin" />
              </div>
              <span class="div-flex-center-end">LinkedIn</span>
            </a>
          </div>
        </div>
        <!-- fim -->
        <div class="links-content-body">
          <div class="links-content card">
            <a href="https://meuevento.tech" target="_blank" class="nuxt-links">
              <div class="div-img img-content">
                <img src="@/assets/img/tela-meuevento.png" alt="github" />
              </div>
              <span class="div-flex-center-end">Api-next</span>
            </a>
          </div>
        </div>
        <!-- fim -->
        <div class="links-content-body">
          <div class="links-content card">
            <a href="https://www.instagram.com/gabriel.fernandes.f/" target="_blank" class="nuxt-links">
              <div class="div-img img-content">
                <img src="@/assets/img/setup.png" alt="github" />
              </div>
              <span class="div-flex-center-end">Instagram</span>
            </a>
          </div>
        </div>
        <!-- fim -->
        <div class="links-content-body">
          <div class="links-content card">
            <a href="https://gabrielfernandes87f.github.io/my-pages/" target="_blank" class="nuxt-links">
              <div class="div-img img-content">
                <img src="@/assets/img/setup.png" alt="github" />
              </div>
              <span class="div-flex-center-end">Git page</span>
            </a>
          </div>
        </div>
        <!-- fim -->
        <div class="links-content-body">
          <div class="links-content card">
            <a href="https://github.com/Gabrielfernandes87f/patins"
             target="_blank" class="nuxt-links">
              <div class="div-img img-content">
                <img src="@/assets/img/setup.png" alt="github" />
              </div>
              <span class="div-flex-center-end">Laravel - patins</span>
            </a>
          </div>
        </div>
        <!-- fim -->
        <div class="links-content-body">
          <div class="links-content card">
            <a href="https://github.com/Gabrielfernandes87f" target="_blank" class="nuxt-links">
              <div class="div-img img-content">
                <img src="@/assets/img/setup.png" alt="github" />
              </div>
              <span class="div-flex-center-end">Meu Github</span>
            </a>
          </div>
        </div>
        <!-- fim -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      name: "Gabriel Fernandes",
      desccription: "Desenvolvedor fullstack web",
      desccription2: " PHP - Laravel - VueJs - NuxtJs - SQL ",
      msg: "A persistência é o caminho do êxito.",
      contentText: "Resolvendo problemas digitais de empresários ou instiuições no que tange a propagações das informações sobre seus negócios e suas atividades. visando a captação de novos clientes e aumentando os lucros, ao mesmo tempo que ajuda a melhorar a qualidade de vida dos seus usuários.",
    };
  },
};
</script>
