<template>
  <div>
    <div class="links-content card">
      <a :href="hrefCard" target="_blank" class="nuxt-links">
        <div class="div-img img-content">

             <img :src="srcCard" :alt="altCard" />
        </div>
        <span class="div-flex-center-end">{{nameCard}}</span>
      </a>
    </div>
  </div>
</template>

<script>
    export default {
    name: "Card",
    data() {
        return {


      }
  },
    props: {
        srcCard: {
            type: String,
            default: '../_nuxt/assets/img/linkedin.png'
      },
        altCard: {
            type: String,
            required: true
      },
        nameCard: {
            type: String,
            required: true
      },

    }
}
</script>
