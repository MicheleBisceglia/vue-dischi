<template>
  <div class="ms_container">
    <AppSelect @selectClick="saveGenre($event)"/>
    <div class="container">
      <div class="row row-cols-3 row-col-md-5 row-col-sd-3 gy-2">
        <AppAlbumCard v-for="item in filterCards()" :key="item.index" :card="item" />
      </div>
    </div>
  </div>
</template>

<script>
import AppAlbumCard from "../components/AppAlbumCard.vue";
import AppSelect from "../components/AppSelect.vue";
import axios from "axios";

export default {
  name: "AppAlbumList",
  components: {
    AppAlbumCard,
    AppSelect
  },
  data: function () {
    return {
      cards: [],
      select: ""
    };
  },
  created() {
    axios
      .get("https://flynn.boolean.careers/exercises/api/array/music")
      .then((resp) => {
        this.cards = resp.data.response;
      });
  },
  methods: {
    saveGenre: function(selectKey) {
      this.select = selectKey;
    },
    filterCards: function() {
    const filteredCards = this.cards.filter( item => {
      return item.genre.includes(this.select)
    });
    return filteredCards;
    }
  }
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
