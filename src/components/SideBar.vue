<template>
  <div id="SideBar">
    <div class="my-image-container">
      <span class="image"></span>
    </div>
    <div class="content-wrapper">
      <div class="header-container">
        <span class="header-text0">
          Hey there!
        </span>
        <span class="header-text1">
          Let's get started.
        </span>
        <span class="subheader-text">
          Tell me a little bit about yourself.
        </span>
      </div>
      <Typeform/>
      <div class="footer-container">
        <span class="footer-text">
          Thanks Gian, chat soon!
        </span>
      </div>
      <button class="submit-button">
        <span class="button-label">
          Submit
        </span>
      </button>
    </div>
  </div>
</template>

<script>
import Typeform from "@/components/Typeform";

export default {
  name: "SideBar",
  components: {
    Typeform,
  }
}
</script>

<style lang="scss" scoped>

#SideBar{
  border-radius: 12px;
  background-color: white;
  box-shadow: 0 4px 22px 1px rgba(73, 74, 95, 0.1);
  display: flex;
  flex-direction: column;

  .my-image-container{
    display: flex;
    align-items: center;
    flex-direction: row-reverse;
    justify-content: space-between;
    width: 100%;
    height: 55px;

    .image{
      width: 55px;
      height: 100%;
      border-radius: 10px;
      background-color: #f6f6f6;
    }
  }
  .content-wrapper{
    display: flex;
    flex-direction: column;
    width: 80%;
    height: fit-content;
    padding-top: 45px;
    margin: 0 auto;

    .header-container{
      padding-left: 5px;
      display: flex;
      flex-direction: column;
      height: 105px;

      .header-text0{
        font-family: "Gilroy SemiBold", serif;
        font-size: 16px;
        color: #1f1f1f;
        letter-spacing: 0;
        line-height: 1.2;
      }

      .header-text1{
        font-family: "Gilroy SemiBold", serif;
        font-size: 26px;
        color: #1f1f1f;
        letter-spacing: 0;
        line-height: 1.2;
      }
      .subheader-text{
        padding-top: 24px;
        font-family: "Bw Modelica Light", serif;
        font-size: 13px;
        color: #4a4a4a;
        letter-spacing: 0;
        line-height: 1.2;
      }
    }
    #Typeform{
      height: 440px;
    }
    .footer-container{
      padding-left: 5px;
      padding-top: 5px;
      display: flex;
      flex-direction: column;
      height: 60px;

      .footer-text{
        font-family: "Bw Modelica Light", serif;
        font-size: 13px;
        color: #1f1f1f;
      }
    }
    .submit-button{
      margin-top: 15px;
      margin-left: auto;
      text-decoration: none;
      outline: none;
      border: 0;
      height: 37px;
      width: 45%;
      background-color: #1f1f1f;
      border-radius: 7px;
      cursor: pointer;

      .button-label{
        font-family: "Bw Modelica Medium", serif;
        font-size: 11px;
        color: white;
      }
    }
  }
}

</style>