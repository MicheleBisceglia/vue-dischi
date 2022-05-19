<template>
  <section>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
  </section>
</template>

<script>
export default {
  name: "AppAlbumCard",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
section {
  display: flex;
  flex-wrap: wrap;
  min-width: 800px;
}
div {
  width: calc(100% / 7);
  margin: 20px;
  height: 200px;//debug
  background-color: $secondary-color;
}
</style>