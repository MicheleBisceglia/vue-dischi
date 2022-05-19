<template>
  <div class="ms_container">
    <div class="container">
        <div class="row row-cols-3 row-col-md-5 row-col-sd-3 gy-2">
            <AppAlbumCard v-for="item in cards" :key="item.index" :card="item" />
        </div>
      
    </div>
  </div>
</template>

<script>
import AppAlbumCard from "../components/AppAlbumCard.vue";
import axios from "axios";

export default {
  name: "AppAlbumList",
  components: {
    AppAlbumCard,
  },
  data: function () {
    return {
      cards: [],
    };
  },
  created() {
    axios
      .get("https://flynn.boolean.careers/exercises/api/array/music")
      .then((resp) => {
        this.cards = resp.data.response;
      });
  },
};
</script>

<style lang="scss">
@import "../style/variables.scss";
.ms_container {
  width: 70%;
  margin: 0 auto;
  margin-top: 50px;
  margin-bottom: 50px;
}
</style>
