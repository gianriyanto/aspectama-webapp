<template>
  <div id="TopBar">
    <span class="logo"></span>
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
  height: 70px;
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

  .myCard-button{
    text-decoration: none;
    outline: none;
    height: 40px;
    width: 120px;
    background-color: transparent;
    border: thin solid #1f1f1f;
    border-radius: 9px;
    cursor: pointer;

    .button-label{
      font-family: "Bw Modelica Bold", serif;
      font-size: 11px;
      color: #1f1f1f;
    }
  }
}

</style>