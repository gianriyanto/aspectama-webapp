<template>
  <div id="MosaicTiles">
    <div class="left-section">
      <div class="left-side">

        <transition appear name="slide-fade-down">
          <span class="card-0">
            <span class="label">
              People-oriented consulting.
            </span>
            <img class="image drop-shadow" src="@/assets/images/timeline.svg" alt="">
          </span>
        </transition>

        <transition appear name="slide-fade-right">
          <span class="card-1">
          <span class="label">
            Your passion at the heart of every decision.
          </span>
          <img class="image drop-shadow" src="@/assets/images/artificial_intelligence.svg" alt="">
        </span>
        </transition>

      </div>
      <div class="right-side">

        <transition appear name="slide-fade-up">
          <span class="card-2">
          <span class="label">
            Free Consultation and Talent Discovery Test.
          </span>
          <img class="image drop-shadow" src="@/assets/images/report_analysis_-2.svg" alt="">
        </span>
        </transition>

      </div>
    </div>
    <div class="right-section">
      <div class="top-side">

        <transition appear name="slide-fade-down">
          <span class="card-3">
          <span class="label">
            Study at institutions around the world.
          </span>
          <img class="image drop-shadow" src="@/assets/images/world_connection_.svg" alt="">
        </span>
        </transition>

        <transition appear name="slide-fade-right">
          <span class="card-4">
          <span class="label">
            Your Future Simplified
          </span>
          <img class="image drop-shadow" src="@/assets/images/graduation.svg" alt="">
        </span>
        </transition>

      </div>
      <div class="bottom-side">

        <transition appear name="slide-fade-left">
          <span class="card-5">
          <span class="label">
            End-to-end solutions tailored to every unique learning journey.
          </span>
          <img class="image drop-shadow" src="@/assets/images/profile_analysis_.svg" alt="">
        </span>
        </transition>

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

@import "/src/styles/animations.scss";

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
        flex-direction: column-reverse;
        justify-content: center;
        height: 40%;
        margin: 0 4px 4px 0;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #fdc0c0, #ffb3c1);

        .label{
          text-align: center;
          padding-top: 5px;
          padding-bottom: 5px;
          font-family: "Gilroy Bold", serif;
          font-size: 14px;
          line-height: 1.3;
          color: #1f1f1f;
          width: 75%;
          align-self: center;
        }
        .image{
          width: 40%;
          align-self: center;
          height: auto;
        }
      }
      .card-1{
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        height: 57%;
        margin: 4px 4px 0 0;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #5da1f3, #708efa);

        .label{
          padding: 15px 20px 0 20px;
          height: fit-content;
          width: 80%;
          font-family: "Gilroy Bold", serif;
          font-size: 16px;
          line-height: 1.3;
          color: white;
        }
        .image{
          margin-left: auto;
          height: 80px;
          width: 80%;
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
          padding: 0 20px 20px 20px;
          height: fit-content;
          font-family: "Gilroy Bold", serif;
          font-size: 20px;
          letter-spacing: -1px;
          line-height: 1.4;
          color: #1f1f1f;
        }

        .image{
          height: 170px;
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
      height: 54%;

      .card-3{
        display: flex;
        flex-direction: column;
        justify-content: center;
        margin: 0 4px 4px 4px;
        width: 55%;
        border-radius: 6px;
        background-image: linear-gradient(to left bottom, #78c2f3, #69a6f1);

        .label{
          padding: 20px 0 5px 0;
          align-self: center;
          text-align: center;
          width: 80%;
          font-family: "Gilroy Bold", serif;
          font-size: 13px;
          letter-spacing: -0px;
          line-height: 1.3;
          color: black;
        }
        .image{
          margin: 0 auto;
          width: 76%;
          height: 90px;
        }
      }
      .card-4{
        display: flex;
        flex-direction: column-reverse;
        justify-content: center;
        margin: 0 0 4px 4px;
        width: 45%;
        border-radius: 6px;
        background-image: linear-gradient(to right top, #2b2b2b, #2d2d2d);

        .label{
          padding: 5px 20px 10px 20px;
          text-align: right;
          font-family: "Gilroy Bold", serif;
          font-size: 16px;
          letter-spacing: 0;
          line-height: 1.2;
          color: #fffae8;
        }
        .image{
          margin: 0 auto;
          align-self: center;
          width: 70%;
          height: 70px;
        }
      }
    }
    .bottom-side{
      display: flex;
      height: 47%;

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
          font-size: 16px;
          line-height: 1.3;
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

  .drop-shadow{
    filter: drop-shadow(1px 10px 15px rgba(96, 88, 88, 0.3));
  }
}


</style>