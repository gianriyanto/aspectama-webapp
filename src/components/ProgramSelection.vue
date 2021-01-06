<template>
  <div id="ProgramSelection">
    <span class="header-text">
      Pick a program level
    </span>
    <div class="selection-container">
      <span class="program-card green-bg">
        <span class="label">
          Foundation
        </span>
        <span class="label">
          College
        </span>
      </span>
      <span class="program-card blue-bg">
        <span class="label">
          Under
        </span>
        <span class="label">
          Graduate
        </span>
      </span>
      <span class="program-card black-bg">
        <span class="label">
          Post
        </span>
        <span class="label">
          Graduate
        </span>
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProgramSelection"
}
</script>

<style lang="scss" scoped>

#ProgramSelection{
  display: flex;
  flex-direction: column;
  align-self: center;

  .header-text{
    font-family: "Bw Modelica Bold", serif;
    font-size: 13px;
    color: #4a4a4a;
    padding-left: 0;
    height: fit-content;
  }

  .selection-container{
    padding-top: 10px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 100%;
    flex-grow: 1;

    .program-card{
      padding: 11px;
      width: 24.5%;
      border-radius: 6px;
      display: flex;
      flex-direction: column;
      text-align: left;

      .label{
        font-family: "Bw Modelica Bold", serif;
        color: white;
        line-height: 1.4;
        font-size: 11px;
      }
    }

    .blue-bg{
      background-color: #7fb9f8;
    }
    .green-bg{
      background-color: #71cbb8;
    }
    .black-bg{
      background-color: #393939;
    }
  }

}

</style>