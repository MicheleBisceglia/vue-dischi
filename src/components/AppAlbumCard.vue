<template>
  <div class="ms_card">
      <div>
        <img :src="card.poster" alt="" />
        <strong class="album-title">{{ card.title }}</strong>
        <small class="album-text">{{ card.author }}</small>
        <small class="album-text">{{ card.year }}</small>
      </div>
  </div>
</template>

<script>
export default {
  name: "AppAlbumCard",
  props: {
    card: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/common.scss";
.ms_card {
  width: calc(100% / 7);
  margin: 20px;
  background-color: $secondary-color;
  text-align: center;
}
</style>
