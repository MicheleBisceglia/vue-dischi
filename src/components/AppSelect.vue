<template>
<select @change="$emit('selectClick',albumSelect)" name="genere" v-model="albumSelect" id="">
      <option value="rock">Rock</option>
      <option value="pop">Pop</option>
      <option value="jazz">Jazz</option>
      <option value="metal">Metal</option>
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

<style lang="scss">
@import "../style/common.scss";
</style>
