<template>
  <div>
    <div class="inner-addon right-addon" id="show_hide_password">
      <label id="label" for>{{nombre}}</label>
      <input type="password" id="password" class="form-control" aria-describedby="button-addon2" />
      <a href class="icone">
        <img class src="~/assets/img/hide.svg" />
      </a>
    </div>
  </div>
</template>


<script>
export default {
  props: ["nombre"]
};
</script>

<style scoped>
label {
  font-size: 12px;
  margin-bottom: 0px;
}
.icone img {
  width: 23px;
  height: 23px;
}
.inner-addon {
  position: relative;
}
.inner-addon .icone {
  position: absolute;
  padding: 10px;
  /* pointer-events: none; */
}
.right-addon .icone {
  background-size: contain;
  border: none;
  outline: none;
  margin-top: 0px;

  z-index: 2;
  opacity: 0.3;
  right: 0px;
  top: 20px;
}
.right-addon input {
  padding-right: 30px;
}
</style>