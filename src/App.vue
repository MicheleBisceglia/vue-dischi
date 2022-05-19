<template>
  <div id="app">
    <body>
      <AppHeader />
      <main>
        <AppAlbumList />
      </main>
    </body>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppAlbumList from "./components/AppAlbumList.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppAlbumList,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
