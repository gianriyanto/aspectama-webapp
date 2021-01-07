<template>
  <div id="ProgramSelection">
    <span class="header-text">
      Pick a program level
    </span>
    <div class="selection-container">
      <span v-for="program in programs"
            v-bind:key=program.index
            class="program-card"
            v-bind:class="{ 'selected-program-card': program.isSelected }"
            @click="selectProgram(program.programName)">
        <span class="label">
          {{ program.programName }}
        </span>
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProgramSelection",
  props: ['selectionData'],
  data() {
    return {
      programs: this.selectionData,
      cardStyle: ['blue-card', 'red-card', 'black-card']
    }
  },
  methods: {
    selectProgram: function(selectedProgram) {
      for (let i = 0; i < this.programs.length; i++) {
        this.programs[i].isSelected = selectedProgram === this.programs[i].programName;
      }
    }
  }
}
</script>

<style lang="scss" scoped>

#ProgramSelection{
  display: flex;
  flex-direction: column;
  align-self: center;

  .header-text{
    padding-left: 2px;
    font-family: "Bw Modelica Bold", serif;
    font-size: 13px;
    color: #4a4a4a;
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
      cursor: pointer;
      padding: 11px;
      width: 23%;
      border-radius: 9px;
      display: flex;
      flex-direction: column;
      text-align: left;
      background-color: #303030;
      border: thin solid #303030;
      transition: all .35s ease-in-out;

      .label{
        font-family: "Bw Modelica Bold", serif;
        color: white;
        line-height: 1.4;
        font-size: 11px;
      }

      &:hover{
        opacity: 0.9;
      }
    }

    .selected-program-card{
      opacity: 1;
      background-color: #69a7f1;
      border: thin solid #69a7f1;
    }
  }

}

</style>