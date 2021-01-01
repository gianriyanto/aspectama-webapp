<template>
  <section id="Home">
    <div class="content-wrapper">
      <div class="header-container">
        <span class="header-text">
          Hi, I'm Ervina.
        </span>
        <span class="header-text">
          Aspectama's education consultant.
        </span>
      </div>
    </div>
    <div id="Typeform">

    </div>
  </section>
</template>

<script>
export default {
  name: "Home"
}
</script>

<style lang="scss" scoped>

#Home{
  display: flex;
  flex-direction: row;
  width: 100%;
  height: 100vh;

  .content-wrapper{
    width: 65%;
    height: 100vh;
    background-color: #2B2B2B;
    border-radius: 0 45px 45px 0;
    box-shadow: 0 0 32px 15px #d6d6d6;
    display: flex;
    flex-direction: column;
    justify-content: center;

    .header-container{
      display: flex;
      flex-direction: column;
      margin: 0 auto;
      height: 550px;
      width: 500px;

      .header-text{
        font-family: "Bw Modelica Medium", serif;
        word-spacing: -0.5px;
        font-size: 40px;
        color: white;
      }
    }
  }
  #Typeform{
    width: 35%;

  }
}

</style>