<template>
  <div id="ContactBar">
    <div class="bar-container">
      <span class="input-label">
        Your contact phone or email
      </span>
      <button class="send-button">
        <span class="button-label">
          Keep in touch
        </span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactBar"
}
</script>

<style lang="scss" scoped>

#ContactBar{
  display: flex;
  justify-content: center;

  .bar-container{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    height: 30px;
    width: 100%;
    border-radius: 50px;
    padding: 3px;
    align-items: center;
    background-color: white;
    box-shadow: 0 5px 25px 1px rgba(77, 79, 109, 0.2);

    .input-label{
      font-family: "Bw Modelica Medium", serif;
      font-size: 12px;
      color: lightgrey;
      letter-spacing: 0;
      padding-left: 15px
    }
    .send-button{
      text-decoration: none;
      outline: none;
      border: 0;
      height: 100%;
      width: 100px;
      background-color: #1f1f1f;
      border-radius: 32px;
      cursor: pointer;

      .button-label{
        font-family: "Bw Modelica Regular", serif;
        font-size: 10px;
        color: white;
      }
    }
  }
}

</style>