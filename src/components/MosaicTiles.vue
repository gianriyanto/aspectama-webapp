<template>
  <div id="MosaicTiles">
    <div class="left-section">
      <div class="left-side">
        <span class="card-0">
          <span class="label">
            Lorem Ipsum
          </span>
        </span>
        <span class="card-1">
          <span class="label">
            Lorem Ipsum
          </span>
        </span>
      </div>
      <div class="right-side">
        <span class="card-2">
          <span class="label">
            Lorem Ipsum
          </span>
        </span>
      </div>
    </div>
    <div class="right-section">
      <div class="top-side">
        <span class="card-3">
          <span class="label">
            Lorem Ipsum
          </span>
        </span>
        <span class="card-4">
          <span class="label">
            Lorem Ipsum
          </span>
        </span>
      </div>
      <div class="bottom-side">
        <span class="card-5">
          <span class="label">
            Lorem Ipsum
          </span>
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
  border-radius: 12px;

  .left-section{
    display: flex;
    flex-direction: row;
    width: 57%;
    height: 100%;

    .left-side{
      display: flex;
      flex-direction: column;
      height: 100%;
      width: 52%;

      .card-0{
        height: 37%;
        padding: 20px;
        margin: 0 3px 3px 0;
        border-radius: 5px;
        background-color: #94baff;

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
        }
      }
      .card-1{
        height: 63%;
        padding: 20px;
        margin: 3px 3px 0 0;
        border-radius: 7px;
        background-color: #9c8ae3;

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
        }
      }
    }
    .right-side{
      display: flex;
      height: 100%;
      width: 48%;

      .card-2{
        margin: 0 3px 0 3px;
        padding: 20px;
        width: 100%;
        border-radius: 7px;
        background-color: #ffda99;

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
        }
      }
    }
  }
  .right-section{
    display: flex;
    flex-direction: column;
    width: 43%;
    height: 100%;

    .top-side{
      display: flex;
      flex-direction: row;
      height: 53%;

      .card-3{
        margin: 0 3px 3px 3px;
        padding: 20px;
        width: 60%;
        border-radius: 7px;
        background-color: #6ea1ff;

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
        }
      }
      .card-4{
        margin: 0 0 3px 3px;
        padding: 20px;
        width: 40%;
        border-radius: 7px;
        background-color: #7bcfd2;

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
        }
      }
    }
    .bottom-side{
      display: flex;
      height: 47%;

      .card-5{
        margin: 3px 0 0 3px;
        padding: 20px;
        width: 100%;
        border-radius: 7px;
        background-color: #8de2cc;

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
        }
      }
    }
  }
}

</style>