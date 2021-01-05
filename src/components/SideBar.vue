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
      <div class="button-container">
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
  components: {
    Typeform,
  }
}
</script>

<style lang="scss" scoped>

#SideBar{
  display: flex;
  flex-direction: column;
  border-radius: 12px;
  background: rgba( 255, 255, 255, 0.15 );
  box-shadow: 0 8px 32px 0 rgba(82, 83, 103, 0.1);
  backdrop-filter: blur( 4px );
  -webkit-backdrop-filter: blur( 4px );

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
    width: 87%;
    height: 100%;
    padding-top: 25px;
    margin: 0 auto;

    .header-container{
      padding-left: 5px;
      display: flex;
      flex-direction: column;
      height: 91px;

      .header-text0{
        font-family: "Gilroy SemiBold", serif;
        font-size: 16px;
        color: #1f1f1f;
        letter-spacing: 0;
        line-height: 1.2;
      }

      .header-text1{
        font-family: "Gilroy SemiBold", serif;
        font-size: 24px;
        color: #1f1f1f;
        letter-spacing: 0;
        line-height: 1.2;
      }

      .subheader-text{
        padding-top: 5px;
        font-family: "Bw Modelica Light", serif;
        font-size: 12px;
        color: #4a4a4a;
        letter-spacing: 0;
        line-height: 1.2;
      }
    }
    #Typeform{
      padding-top: 5px;
      height: fit-content;
    }
    .footer-container{
      padding-left: 5px;
      padding-top: 5px;
      display: flex;
      flex-direction: column;
      height: 50px;

      .footer-text{
        font-family: "Bw Modelica Light", serif;
        font-size: 13px;
        color: #1f1f1f;
      }
    }
    .button-container{
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
      flex-grow: 1;

      .submit-button{
        margin-left: auto;
        height: 40px;
        width: 41%;
        background-color: #1f1f1f;
        border-radius: 8px;

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