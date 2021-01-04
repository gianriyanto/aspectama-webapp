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
        box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.25 );
        background-image: linear-gradient(to right top, #97d1f8, #94c7fd, #99bcff, #a7affe, #baa0f6);

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
        box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.35 );
        background-image: linear-gradient(to right top, #777cee, #857ceb, #927de8, #9c7ee4, #a67fe1);
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
        background-image: linear-gradient(to right top, #b19bf0, #f299d5, #ffa5b3, #ffbd9b, #ffda99);

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
        box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.15 );
        background-image: linear-gradient(to left bottom, #fb899c, #ff978e, #ffa884, #febb7f, #f4cd83);

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
        box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.15 );
        background-image: linear-gradient(to right top, #fb7e7e, #fe88a6, #f697ca, #e6aae7, #d2bcfb);

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
        box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
        background-image: linear-gradient(to right top, #89d5b1, #45d5de, #48ccff, #a9b7ff, #f99ae9);

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
        }
      }
    }
  }
}

</style>