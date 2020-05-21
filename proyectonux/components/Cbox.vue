<template>
  <label class="custom-radio-checkbox">
    <input class="custom-radio-checkbox__input" type="checkbox" />
    <span class="custom-radio-checkbox__show custom-radio-checkbox__show--checkbox"></span>
    {{contenido}}
  </label>
</template>

<script>
export default {
  props: ["contenido"]
};
</script>


<style scoped>
.custom-radio-checkbox span {
  border: 1px solid;
}
.custom-radio-checkbox {
  display: inline-flex;
  align-items: center;
  cursor: pointer;
  font-size: 12px;
  margin-bottom: 0px;
}

/* Modificador para dar la imagen de checkbox */
.custom-radio-checkbox__show--checkbox {
  background-image: none;
}

/* Oculta input original */
.custom-radio-checkbox > .custom-radio-checkbox__input {
  display: none;
}

/* Radio personalizado usando <span> */
.custom-radio-checkbox > .custom-radio-checkbox__show {
  display: inline-block;
  width: 15px;
  height: 15px;
  margin-right: 0.5rem;
  background-size: cover;
}

/* Cambia el checkbox personalizado cuando es pulsado */
.custom-radio-checkbox
  > .custom-radio-checkbox__input:checked
  + .custom-radio-checkbox__show--checkbox {
  background-image: url("~static/img/check_for_checkbox.svg");
}
</style>