<template>
  <div class="container">
      <div class="ms_container">
          <AppAlbumCard />
      </div>
  </div>
</template>

<script>
import AppAlbumCard from "../components/AppAlbumCard.vue";
export default {
  name: "AppAlbumList",
  components: {
      AppAlbumCard
  }
};
</script>

<style lang="scss">
@import "../style/variables.scss";
.ms_container {
    width: 70%;
    margin: 0 auto;
    margin-top: 50px;
}
</style>
