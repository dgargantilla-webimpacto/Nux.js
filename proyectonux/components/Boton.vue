<template>
  <button type="button" class="btn btn-primary btn-block">{{contenido}}</button>
</template>

<script>
export default {
  props: ["contenido"]
};
</script>

<style scoped>
button {
  background-color: #fa2398;
  border-color: #fa2398;
  color: #ffffff;
}
</style>