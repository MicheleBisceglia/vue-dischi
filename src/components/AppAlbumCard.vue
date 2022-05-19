<template>
  <div class="ms_container">
    <div class="ms_card">
      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
      <strong class="album-title">New jersey</strong>
      <small class="album-text">Bon Jovi</small>
      <small class="album-text">1988</small>
    </div>
    <div class="ms_card">
      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
      <strong class="album-title">New jersey</strong>
      <small class="album-text">Bon Jovi</small>
      <small class="album-text">1988</small>
    </div>
    <div class="ms_card">
      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
      <strong class="album-title">New jersey</strong>
      <small class="album-text">Bon Jovi</small>
      <small class="album-text">1988</small>
    </div>
    <div class="ms_card">
      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
      <strong class="album-title">New jersey</strong>
      <small class="album-text">Bon Jovi</small>
      <small class="album-text">1988</small>
    </div>
    <div class="ms_card">
      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
      <strong class="album-title">New jersey</strong>
      <small class="album-text">Bon Jovi</small>
      <small class="album-text">1988</small>
    </div>
    <div class="ms_card">
      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
      <strong class="album-title">New jersey</strong>
      <small class="album-text">Bon Jovi</small>
      <small class="album-text">1988</small>
    </div>
    <div class="ms_card">
      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
      <strong class="album-title">New jersey</strong>
      <small class="album-text">Bon Jovi</small>
      <small class="album-text">1988</small>
    </div>
    <div class="ms_card">
      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
      <strong class="album-title">New jersey</strong>
      <small class="album-text">Bon Jovi</small>
      <small class="album-text">1988</small>
    </div>
    <div class="ms_card">
      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
      <strong class="album-title">New jersey</strong>
      <small class="album-text">Bon Jovi</small>
      <small class="album-text">1988</small>
    </div>
    <div class="ms_card">
      <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
      <strong class="album-title">New jersey</strong>
      <small class="album-text">Bon Jovi</small>
      <small class="album-text">1988</small>
    </div>

  </div>
</template>

<script>
export default {
  name: "AppAlbumCard",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/common.scss";
.ms_container {
  display: flex;
  flex-wrap: wrap;
  min-width: 800px;
}
.ms_card {
  width: calc(100% / 7);
  margin: 20px;
  height: 200px;//debug
  background-color: $secondary-color;
  text-align: center;
}
</style>