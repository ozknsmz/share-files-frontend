<template>
  <div class="peers-file">
    <v-file-input
      hide-input
      multiple
      show-size
      truncate-length="15"
      prepend-icon="mdi-access-point"
    ></v-file-input>
  </div>
</template>
<script>
export default {
  name: "UserIcon",

  data: () => ({}),
};
</script>




<style scoped>
.peers-file {
  display: flex;
  justify-content: center;
  align-items: center;
}

.v-icon.v-icon {
  font-size: 40px !important;
}
</style>
