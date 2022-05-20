<template>
  <div>
    <header>
      <div class="ms_logo">
        <img src="../assets/logo-small.svg" alt="" />
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style scoped lang="scss">
@import "../style/variables.scss";
header {
  height: 70px;
  background-color: $secondary-color;
  .ms_logo {
    height: 60px;
    width: 60px;
    margin-left: 10px;
  }
}
</style>
