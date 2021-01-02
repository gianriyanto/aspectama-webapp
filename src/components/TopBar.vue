<template>
  <div id="TopBar">
    <span class="logo">

    </span>
    <button class="mycard-button">
      <span class="button-label">
        Take my Card
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
  width: 100%;
  height: 70px;
  border: thin solid darkorange;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  .logo{
    width: 25px;
    height: 50px;
    background-color: #1f1f1f;
    border-bottom-left-radius: 25px;
    border-top-left-radius: 25px;
  }

  .mycard-button{
    text-decoration: none;
    outline: none;
    height: 46px;
    width: 120px;
    background-color: transparent;
    border: thin solid black;
    border-radius: 9px;

    .button-label{
      font-family: "Bw Modelica Medium", serif;
      font-size: 12px;
      color: black;
    }
  }
}

</style>