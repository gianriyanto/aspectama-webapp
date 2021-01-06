<template>
  <div id="MosaicTiles">
    <div class="left-section">
      <div class="left-side">
        <span class="card-0">
          <span class="label">
          </span>
        </span>
        <span class="card-1">
          <span class="label">
          </span>
        </span>
      </div>
      <div class="right-side">
        <span class="card-2">
          <span class="label">
          </span>
        </span>
      </div>
    </div>
    <div class="right-section">
      <div class="top-side">
        <span class="card-3">
          <span class="label">
          </span>
        </span>
        <span class="card-4">
          <span class="label">
          </span>
        </span>
      </div>
      <div class="bottom-side">
        <span class="card-5">
          <span class="label">
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
      width: 51%;

      .card-0{
        display: flex;
        flex-direction: row-reverse;
        height: 37%;
        padding: 15px 20px;
        margin: 0 4px 4px 0;
        border-radius: 6px;
        background-image: linear-gradient(to left bottom, #97d1f8, #94c7fd, #99b6ff);

        .label{
          margin-top: auto;
          font-family: "Bw Modelica ExtraBold", serif;
          font-size: 18px;
          letter-spacing: -1px;
          line-height: 1.3;
          color: #1f1f1f;
        }
      }
      .card-1{
        display: flex;
        flex-direction: column-reverse;
        height: 63%;
        padding: 15px 20px;
        margin: 4px 4px 0 0;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #b9a6ff, #a5afff);

        .label{
          width: 60%;
          font-family: "Bw Modelica ExtraBold", serif;
          font-size: 18px;
          letter-spacing: -0.5px;
          line-height: 1.3;
          color: #1f1f1f;
        }
      }
    }
    .right-side{
      display: flex;
      height: 100%;
      width: 49%;

      .card-2{
        display: flex;
        flex-direction: column-reverse;
        margin: 0 4px 0 4px;
        padding: 15px 20px;
        width: 100%;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #fad7b8, #fdd690);

        .label{
          width: 50%;
          font-family: "Bw Modelica ExtraBold", serif;
          font-size: 20px;
          letter-spacing: -1px;
          line-height: 1.2;
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
      height: 57%;

      .card-3{
        display: flex;
        flex-direction: row-reverse;
        margin: 0 4px 4px 4px;
        padding: 15px 20px;
        width: 60%;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #74b3ff, #8da6ff);

        .label{
          text-align: right;
          width: 50%;
          font-family: "Bw Modelica ExtraBold", serif;
          font-size: 16px;
          letter-spacing: -0.5px;
          line-height: 1.2;
          color: #1f1f1f;
        }
      }
      .card-4{
        display: flex;
        flex-direction: column-reverse;
        margin: 0 0 4px 4px;
        padding: 15px 20px;
        width: 40%;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #fd8f8f, #ff96a9);

        .label{
          text-align: right;
          font-family: "Bw Modelica ExtraBold", serif;
          font-size: 14px;
          letter-spacing: -0.5px;
          line-height: 1.2;
        }
      }
    }
    .bottom-side{
      display: flex;
      height: 43%;

      .card-5{
        display: flex;
        margin: 4px 0 0 4px;
        padding: 15px 20px;
        width: 100%;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #a5dec3, #a9e5e7);

        .label{
          margin: auto;
          text-align: center;
          font-family: "Bw Modelica ExtraBold", serif;
          font-size: 23px;
          letter-spacing: -0.5px;
          line-height: 1.2;
          color: #1f1f1f;
        }
      }
    }
  }
}

</style>