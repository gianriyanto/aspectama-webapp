<template>
  <div id="Typeform">
    <div class="input-card">
      <span class="prompt">
        Let's get started with your name
      </span>
      <span class="input">
        Your full name
        <check-circle-icon size="1x" class="icon"></check-circle-icon>
      </span>
    </div>
    <div class="input-card">
      <span class="prompt">
        What would you like to study
      </span>
      <span class="input">
        Interested major or course
        <check-circle-icon size="1x" class="icon"></check-circle-icon>
      </span>
    </div>
    <div class="input-card">
      <span class="prompt">
        You'd like to travel to study at
      </span>
      <span class="input">
        City or Country
        <check-circle-icon size="1x" class="icon"></check-circle-icon>
      </span>
    </div>
    <div class="input-card">
      <span class="prompt">
        To pursue a career as a
      </span>
      <span class="input">
        Career Profession
        <check-circle-icon size="1x" class="icon"></check-circle-icon>
      </span>
    </div>
    <div class="input-card">
      <span class="prompt">
        Cool! It's best to reach you at
      </span>
      <span class="input">
        Phone or email
        <check-circle-icon size="1x" class="icon"></check-circle-icon>
      </span>
    </div>
  </div>
</template>

<script>
import { CheckCircleIcon } from 'vue-feather-icons'

export default {
  name: "Typeform",
  components: {
    CheckCircleIcon
  }

}
</script>

<style lang="scss" scoped>

 #Typeform{
   display: flex;
   flex-direction: column;
   justify-content: flex-start;

   .input-card{
     display: flex;
     flex-direction: column;
     justify-content: space-evenly;
     padding: 5px 20px;
     width: 85%;
     height: 65px;
     border-radius: 6px;
     border: 1px solid #f3f3f3;
     margin-bottom: 20px;
     background-color: white;
     box-shadow: 0 10px 20px 1px rgba(127, 128, 140, 0.1);

     .prompt {
       font-family: "Bw Modelica Bold", serif;
       font-size: 13px;
       color: #4a4a4a;
     }
     .input{
       font-family: "Bw Modelica Light", serif;
       font-size: 13px;
       color: black;

       .icon{
         padding-left: 3px;
         transform: translateY(2px);
         font-size: 13px;
         color: #16a075;
       }
     }
   }
 }

</style>