<template>
  <div id="CallToAction">
    <button class="contact-button" v-on:click="goToSite('https://wa.me/+6281232012145')">
      <font-awesome-icon class="whatsapp-icon" :icon="['fab', 'whatsapp']" />
      <span class="button-label">
        Contact Me
      </span>
    </button>
    <button class="testimony-button">
      <span class="button-label">
        Client Stories
      </span>
    </button>
  </div>
</template>

<script>

export default {
  name: "CallToAction",
  methods: {
    goToSite(url) {
      window.open(url, '_blank');
    }
  },
}
</script>

<style lang="scss" scoped>

#CallToAction{
  display: flex;
  flex-direction: row;

  .contact-button{
    display: flex;
    flex-direction: row-reverse;
    justify-content: center;
    height: 41px;
    width: 150px;
    background-image: linear-gradient(to right, #128c7e, #128c7e);
    border-radius: 30px;
    transition: all .4s ease-in-out;
    filter: drop-shadow(1px 6px 10px rgba(96, 88, 88, 0.4));

    .whatsapp-icon{
      align-self: center;
      font-size: 20px;
      color: white;
      padding-left: 10px;
    }

    .button-label{
      align-self: center;
      padding-top: 3px;
      font-family: "Gilroy Regular", serif;
      font-size: 12px;
      letter-spacing: 0.3px;
      color: white;
    }

    &:hover{
      opacity: 0.8;
    }
  }
  .testimony-button{
    align-self: center;
    margin-left: 20px;
    height: 41px;
    width: fit-content;
    background-color: transparent;
    border: thin solid transparent;

    .button-label{
      font-family: "Bw Modelica Bold", serif;
      font-size: 14px;
      color: #1f1f1f;
      transition: all .3s ease-in-out;

      &:hover{
        opacity: 0.7;
      }
    }
  }
}

</style>