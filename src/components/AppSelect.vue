<template>
  <select @change="$emit('selectClick',albumSelect)" name="genere" v-model="albumSelect" id="">
    <option value="Rock">Rock</option>
    <option value="Pop">Pop</option>
    <option value="Jazz">Jazz</option>
    <option value="Metal">Metal</option>
  </select>
</template>

<script>
export default {
  name: "AppSelect",
  data: function() {
      return {
          albumSelect: ''
      }
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

</style>
