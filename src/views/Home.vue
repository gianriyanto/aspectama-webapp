<template>
  <section id="Home">
    <div class="content-wrapper">
      <div class="header-container">
        <span class="header-text">
        </span>
      </div>
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
    width: 70%;
    height: 100vh;
    background-image: linear-gradient(to top right, #1f1f1f, #2b2b2b);
    border-radius: 0 25px 25px 0;
    box-shadow: 0 0 32px 15px #d6d6d6;
    display: flex;
    flex-direction: column;
    justify-content: center;

    .header-container{
      display: flex;
      flex-direction: column;
      margin: 0 auto;
      height: fit-content;
      width: 500px;

      .header-text{
        line-height: 1.4;
        font-family: "Bw Modelica Medium", serif;
        word-spacing: -0.5px;
        font-size: 38px;
        color: white;
      }
    }
  }
}

</style>