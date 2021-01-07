<template>
  <div id="TopBar">
    <span class="logo-container">
      <img class="logo-image" src="@/assets/logo/AspectamaLogo.png" alt="">
    </span>
    <button class="myCard-button">
      <span class="button-label">
        Take my card
      </span>
    </button>
  </div>
</template>

<script>
export default {
  name: "TopBar"
}
</script>

<style lang="scss" scoped>

#TopBar{
  width: 95%;
  height: 75px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  .logo-container{
    padding-top: 3px;

    .logo-image{
      height: 55px;
      width: auto;
    }
  }

  .myCard-button{
    height: 42px;
    width: 120px;
    background-color: transparent;
    border: thin solid #1f1f1f;
    border-radius: 9px;

    .button-label{
      font-family: "Bw Modelica Bold", serif;
      font-size: 12px;
      color: #1f1f1f;
    }
  }
}

</style>