<template>
  <div id="MosaicTiles">
    <div class="left-section">
      <div class="left-side">
        <span class="card-0">

        </span>
        <span class="card-1">

        </span>
      </div>
      <div class="right-side">
        <span class="card-2">

        </span>
      </div>
    </div>
    <div class="right-section">
      <div class="top-side">
        <span class="card-3">

        </span>
        <span class="card-4">

        </span>
      </div>
      <div class="bottom-side">
        <span class="card-5">

        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MosaicTiles"
}
</script>

<style lang="scss" scoped>

#MosaicTiles{
  display: flex;
  flex-direction: row;
  width: 65%;
  height: 290px;
  border-radius: 12px;

  .left-section{
    display: flex;
    flex-direction: row;
    width: 55%;
    height: 100%;

    .left-side{
      display: flex;
      flex-direction: column;
      width: 50%;

      .card-0{
        height: 40%;
        margin: 0 3px 3px 0;
        border-radius: 5px;
        background-color: #eaeaea;
      }
      .card-1{
        height: 60%;
        margin: 3px 3px 0 0;
        border-radius: 7px;
        background-color: #eaeaea;
      }
    }
    .right-side{
      display: flex;
      width: 55%;

      .card-2{
        margin: 0 3px 0 3px;
        width: 100%;
        height: 100%;
        border-radius: 7px;
        background-color: #eaeaea;
      }
    }
  }
  .right-section{
    display: flex;
    flex-direction: column;
    width: 50%;
    height: 100%;

    .top-side{
      display: flex;
      flex-direction: row;
      height: 53%;

      .card-3{
        margin: 0 3px 3px 3px;
        width: 60%;
        border-radius: 7px;
        background-color: #eaeaea;
      }
      .card-4{
        margin: 0 0 3px 3px;
        width: 40%;
        border-radius: 7px;
        background-color: #eaeaea;
      }
    }
    .bottom-side{
      display: flex;
      height: 47%;

      .card-5{
        margin: 3px 0 0 3px;
        width: 100%;
        border-radius: 7px;
        background-color: #eaeaea;
      }
    }
  }
}

</style>