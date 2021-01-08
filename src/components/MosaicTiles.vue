<template>
  <div id="MosaicTiles">
    <div class="left-section">
      <div class="left-side">
        <span class="card-0">
          <span class="label">
            End to end consulting service.
          </span>
          <img class="image" src="@/assets/images/timeline.svg" alt="">
        </span>
        <span class="card-1">
          <span class="label">
            Passion and purpose at the centre of every decision.
          </span>
          <img class="image" src="@/assets/images/artificial_intelligence.svg" alt="">
        </span>
      </div>
      <div class="right-side">
        <span class="card-2">
          <span class="label">
            Discover your talent and potential with a free aptitude test.
          </span>
          <img class="image" src="@/assets/images/report_analysis_-2.svg" alt="">
        </span>
      </div>
    </div>
    <div class="right-section">
      <div class="top-side">
        <span class="card-3">
          <span class="label">
            Study at institutions around the world.
          </span>
          <img class="image" src="@/assets/images/world_connection_.svg" alt="">
        </span>
        <span class="card-4">
          <span class="label">
            Your Future Simplified
          </span>
          <img class="image" src="@/assets/images/graduation.svg" alt="">
        </span>
      </div>
      <div class="bottom-side">
        <span class="card-5">
          <span class="label">
            People-oriented solutions tailored to your unique learning journey.
          </span>
          <img class="image" src="@/assets/images/profile_analysis_.svg" alt="">
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
    width: 55%;
    height: 100%;

    .left-side{
      display: flex;
      flex-direction: column;
      height: 100%;
      width: 51%;

      .card-0{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        height: 40%;
        margin: 0 4px 4px 0;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #fdc0c0, #ffb3c1);

        .label{
          padding-left: 15px;
          padding-bottom: 15px;
          padding-top: 15px;
          width: 40%;
          font-family: "Gilroy Bold", serif;
          font-size: 14px;
          line-height: 1.3;
          color: black;
        }
        .image{
          margin-top: auto;
          padding-bottom: 15px;
          padding-right: 10px;
          width: 45%;
          height: auto;
        }
      }
      .card-1{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        height: 57%;
        margin: 4px 4px 0 0;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #5da1f3, #708efa);

        .label{
          padding-top: 15px;
          padding-left: 15px;
          height: 40%;
          width: 80%;
          font-family: "Gilroy Bold", serif;
          font-size: 14px;
          line-height: 1.3;
          color: white;
        }
        .image{
          margin-left: auto;
          height: 54%;
          width: 130px;
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
        justify-content: space-between;
        margin: 0 4px 0 4px;
        width: 100%;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #fadcb8, #fddda7);

        .label{
          padding: 0 20px 15px 20px;
          height: fit-content;
          font-family: "Gilroy Bold", serif;
          font-size: 17px;
          letter-spacing: -0.5px;
          line-height: 1.4;
          color: #1f1f1f;
        }

        .image{
          height: 150px;
          width: 100%;
        }
      }
    }
  }
  .right-section{
    display: flex;
    flex-direction: column;
    width: 45%;
    height: 100%;

    .top-side{
      display: flex;
      flex-direction: row;
      height: 57%;

      .card-3{
        display: flex;
        flex-direction: column;
        justify-content: center;
        margin: 0 4px 4px 4px;
        width: 55%;
        border-radius: 6px;
        background-image: linear-gradient(to left bottom, #78c2f3, #69a6f1);

        .label{
          padding: 10px 20px 5px 20px;
          text-align: center;
          width: fit-content;
          font-family: "Gilroy Bold", serif;
          font-size: 12.5px;
          letter-spacing: -0.3px;
          line-height: 1.3;
          color: white;
        }
        .image{
          margin: 0 auto;
          width: 82%;
          height: fit-content;
        }
      }
      .card-4{
        display: flex;
        flex-direction: column-reverse;
        justify-content: space-between;
        margin: 0 0 4px 4px;
        width: 45%;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #3c3c3c, #474747);

        .label{
          padding: 0 20px 15px 20px;
          text-align: right;
          font-family: "Gilroy Bold", serif;
          font-size: 16px;
          letter-spacing: 0;
          line-height: 1.2;
          color: #fffae8;
        }
        .image{
          padding: 10px 20px 0 10px;
          margin-right: auto;
          align-self: flex-end;
          width: 70%;
          height: fit-content;
        }
      }
    }
    .bottom-side{
      display: flex;
      height: 43%;

      .card-5{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        margin: 4px 0 0 4px;
        width: 100%;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #969bfc, #788df6);

        .label{
          padding: 15px 0 15px 20px;
          margin: auto 0;
          width: 85%;
          text-align: left;
          font-family: "Gilroy Bold", serif;
          font-size: 13px;
          line-height: 1.4;
          color: white;
        }

        .image{
          margin: auto 0;
          height: 100px;
          width: 130px;
        }
      }
    }
  }
}

</style>