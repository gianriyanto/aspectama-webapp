<template>
  <div id="ContactDetails">
    <span class="phone">
      62 812 3201 2145
    </span>
    <span class="slash"> / </span>
    <a class="email" href="mailto:consult@aspectamalsut.co.id">
      consult@aspectamalsut.co.id
    </a>
  </div>
</template>

<script>
export default {
  name: "ContactDetails"
}
</script>

<style lang="scss" scoped>

#ContactDetails{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  .phone{
    font-family: "Gilroy Regular", serif;
    font-size: 13px;
    color: black;
  }

  .email{
    font-family: "Gilroy Regular", serif;
    font-size: 13px;
    color: black;
    cursor: pointer;
    transition: all .35s ease-in-out;

    &:hover{
      opacity: 0.8;
      color: #3389f6;
    }
  }
  .slash{
    font-family: "Gilroy Regular", serif;
    font-size: 13px;
    color: #292929;
  }
}

</style>