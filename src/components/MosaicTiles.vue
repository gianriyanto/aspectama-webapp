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
        background-image: linear-gradient(to right top, #97d1f8, #94c7fd, #99bcff);

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
          color: #1f1f1f;
        }
      }
      .card-1{
        height: 63%;
        padding: 20px;
        margin: 3px 3px 0 0;
        border-radius: 7px;
        box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.35 );
        background-image: linear-gradient(to right top, #777cee, #857ceb, #927de8, #9c7ee4);

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
          color: white;
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
        background-image: linear-gradient(to right top, #b9a6ee, #efb0da, #f6b1bc, #fac3b1, #ffda99);

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
          color: #1f1f1f;
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
        background-image: linear-gradient(to right top, #7e94ff, #898eff, #9687ff, #a380ff, #b177fd);

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
          color: white;
        }
      }
      .card-4{
        margin: 0 0 3px 3px;
        padding: 20px;
        width: 40%;
        border-radius: 7px;
        box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.15 );
        background-image: linear-gradient(to right top, #f87c7c, #fa8189, #fb8796, #fb8da2, #fb94ae);

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
        background-image: linear-gradient(to right top, #91d6b5, #95dadd, #81c6e2);

        .label{
          font-family: "Bw Modelica Bold", serif;
          font-size: 17px;
        }
      }
    }
  }
}

</style>