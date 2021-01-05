<template>
  <div id="Typeform">
    <div class="input-card">
      <span class="prompt">
        Let's start with your name
      </span>
      <span class="input">
        Your full name
        <check-circle-icon size="1x" class="icon"></check-circle-icon>
      </span>
    </div>
    <div class="input-card">
      <span class="prompt">
        And you're looking for a
      </span>
      <span class="input">
        college, undergrad, postgrad?
        <check-circle-icon size="1x" class="icon"></check-circle-icon>
      </span>
    </div>
    <div class="input-card">
      <span class="prompt">
        You're most interested to study
      </span>
      <span class="input">
        Interested major or course
        <check-circle-icon size="1x" class="icon"></check-circle-icon>
      </span>
    </div>
    <div class="input-card">
      <span class="prompt">
        And travel abroad to
      </span>
      <span class="input">
        Preferred city or country?
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
     margin-bottom: 15px;
     display: flex;
     flex-direction: column;
     justify-content: space-evenly;
     padding: 5px 20px;
     width: 85%;
     height: 65px;
     border-radius: 6px;
     border: 1px solid rgba( 255, 255, 255, 0.18 );
     background: rgba( 255, 255, 255, 0.00 );
     box-shadow: 0 3px 15px 0 rgba( 31, 38, 135, 0.1 );
     backdrop-filter: blur( 3.0px );
     -webkit-backdrop-filter: blur( 3.0px );

     .prompt {
       font-family: "Bw Modelica Bold", serif;
       font-size: 12px;
       color: #4a4a4a;
     }
     .input{
       font-family: "Bw Modelica Light", serif;
       font-size: 12px;
       color: #5f5f5f;

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