<template>
  <div id="SideBar">
    <div class="my-image-container">
      <span class="image">

      </span>
    </div>
    <div class="content-wrapper">
      <div class="header-container">
        <span class="header-text">
          Hey there!
        </span>
        <span class="header-text">
          Let's get started.
        </span>
        <span class="subheader-text">
          Start by telling me a little bit about yourself
        </span>
      </div>
      <Typeform/>
      <div class="footer-container">
        <span class="footer-text">
          Thanks Gian, chat soon!
        </span>
        <button class="submit-button">
          <span class="button-label">
            Submit
          </span>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import Typeform from "@/components/Typeform";
export default {
  name: "SideBar",
  components: {Typeform}
}
</script>

<style lang="scss" scoped>

#SideBar{
  border-radius: 12px;
  background-color: white;
  box-shadow: 0 10px 30px 1px rgba(73, 74, 95, 0.15);
  display: flex;
  flex-direction: column;

  .my-image-container{
    display: flex;
    align-items: center;
    flex-direction: row-reverse;
    width: 100%;
    height: 50px;

    .image{
      width: 50px;
      height: 100%;
      border-radius: 10px;
      background-color: lightgrey;
    }
  }
  .content-wrapper{
    display: flex;
    flex-direction: column;
    width: 88%;
    height: fit-content;
    border: thin solid lightgrey;
    padding-top: 50px;
    margin: 0 auto;

    .header-container{
      display: flex;
      flex-direction: column;
      height: 100px;

      .header-text{
        font-family: "Gilroy SemiBold", serif;
        font-size: 25px;
        color: #1f1f1f;
        letter-spacing: 0;
        line-height: 1.2;
      }
      .subheader-text{
        padding-top: 10px;
        font-family: "Gilroy Regular", serif;
        font-size: 14px;
        color: #1f1f1f;
        letter-spacing: 0;
        line-height: 1.2;
      }
    }
    #Typeform{
      height: 450px;
      width: 100%;
      border: thin solid darkslategray;
    }
    .footer-container{
      display: flex;
      flex-direction: column;
      height: 80px;
      border: thin solid green;
      padding-top: 20px;
      align-items: center;

      .footer-text{
        font-family: "Gilroy SemiBold", serif;
        font-size: 17px;
        color: #1f1f1f;
      }
      .submit-button{
        margin-top: 15px;
        text-decoration: none;
        outline: none;
        border: 0;
        height: 36px;
        width: 90%;
        background-color: #1f1f1f;
        border-radius: 32px;
        cursor: pointer;

        .button-label{
          font-family: "Bw Modelica Medium", serif;
          font-size: 11px;
          color: white;
        }
      }
    }
  }
}

</style>