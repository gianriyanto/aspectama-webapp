<template>
  <div id="SideBar">
    <div class="my-image-container">
      <span class="image">
        <span class="label"> ET </span>
      </span>
    </div>
    <div class="content-wrapper">
      <div class="header-container">
        <span class="header-text">
          Let's get started.
        </span>
        <span class="subheader-text">
          Tell me a little bit about yourself.
        </span>
      </div>
      <Typeform id="Typeform"/>
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
  border-radius: 15px;
  background-color: #f6f6f6;
  height: fit-content;

  .my-image-container{
    display: flex;
    align-items: center;
    flex-direction: row-reverse;
    justify-content: space-between;
    align-self: center;
    width: 91%;
    height: 55px;

    .image{
      display: flex;
      width: 55px;
      height: 100%;
      border-radius: 50%;
      background-color: #ececec;

      .label{
        padding-top: 5px;
        padding-left: 2px;
        margin: auto;
        font-family: "Gilroy Bold", serif;
        font-size: 20px;
        letter-spacing: 2px;
        color: #d2d2d2;
      }
    }
  }
  .content-wrapper{
    display: flex;
    flex-direction: column;
    width: 87%;
    height: 100%;
    padding-top: 5px;
    margin: 0 auto;

    .header-container{
      padding-left: 2px;
      display: flex;
      flex-direction: column;
      height: fit-content;

      .header-text{
        font-family: "Bw Modelica Bold", serif;
        font-size: 24px;
        color: #1f1f1f;
        letter-spacing: -1px;
        line-height: 1.2;
      }

      .subheader-text{
        padding-top: 7px;
        font-family: "GIlroy Light", serif;
        font-size: 15px;
        color: #4a4a4a;
        letter-spacing: 0;
        line-height: 1.2;
      }
    }
    #Typeform{
      padding-top: 25px;
      height: fit-content;
      flex-grow: 1;
    }

  }
}

</style>