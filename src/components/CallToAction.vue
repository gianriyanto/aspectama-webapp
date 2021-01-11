<template>
  <div id="CallToAction">
    <button class="contact-button">
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
  components: {
  }
}
</script>

<style lang="scss" scoped>

#CallToAction{
  display: flex;
  flex-direction: row;

  .contact-button{
    height: 42px;
    width: 150px;
    background-image: linear-gradient(to right, #2b2b2b, #3b3b3b);
    border: thin solid #2b2b2b;
    border-radius: 30px;
    transition: all .3s ease-in-out;
    filter: drop-shadow(1px 6px 10px rgba(96, 88, 88, 0.6));

    .button-label{
      font-family: "Bw Modelica Medium", serif;
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
    height: 42px;
    width: fit-content;
    background-color: transparent;
    transition: all .3s ease-in-out;

    .button-label{
      font-family: "Bw Modelica Bold", serif;
      font-size: 13px;
      color: #2b2b2b;
    }

    &:hover{
      opacity: 0.7;
    }
  }
}

</style>