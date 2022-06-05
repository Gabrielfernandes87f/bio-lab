<template>
  <div class="index">
    <div class="body">
      <div class="desk-display">
        <h1>Apenas suporte mobile, abra esse link no seu dispositivo movel</h1>
        <a
          href="https://play.google.com/store/apps/details?id=com.app.tcc.tccapp"
          target="_blank"
        >
          <img
            src="https://play.google.com/intl/en_us/badges/static/images/badges/pt-br_badge_web_generic.png"
            alt="Download Android"
          />
        </a>
      </div>
      <div class="main">
        <div class="main-title">
          <img
            class="avatar-perfil"
            src="@/assets/img/setup.png"
            alt="avatar"
            srcset="@/assets/img/setup.png"
          />
          <h1 class="name">{{ name }}</h1>
          <h2>{{ desccription }}</h2>
          <h3>{{ desccription2 }}</h3>
          <hr />
        </div>
        <div class="content-description">
          <p>{{ msg }}</p>
          <p>{{ contentText }}</p>
        </div>
        <div class="links-content">
          <a
            href="https://github.com/Gabrielfernandes87f"
            target="_blank"
            class="nuxt-links"
          >
            <img src="@/assets/img/setup.png" alt="github" />
            <span>meu github</span>
          </a>
        </div>
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
      desccription2: " PHP - Laravel - Vue - NuxtJs - SQL ",
      msg: "A vida é uma coisa que se pode mudar, mas a mudança é uma coisa que se pode perder.",
      contentText:
        "Sou fotógrafo profissional, Com 8 anos de carreira. hoje trabalho como freelancer, desenvolvendo sites e aplicativos para web",
    };
  },
};
</script>
