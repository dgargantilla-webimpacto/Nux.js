<template>
  <div class="col radio">
    <div>
      <label class="custom-radio-checkbox">
        <!-- Input oculto -->
        <input class="custom-radio-checkbox__input" type="radio" checked />
        <!-- Imagen en sustitucion -->
        <span class="custom-radio-checkbox__show custom-radio-checkbox__show--radio"></span>
        <!-- Texto -->
        <span class="custom-radio-checkbox__text">{{nombre1}}</span>
      </label>
    </div>
    <div>
      <label class="custom-radio-checkbox">
        <!-- Input oculto -->
        <input class="custom-radio-checkbox__input" type="radio" />
        <!-- Imagen en sustitucion -->
        <span class="custom-radio-checkbox__show custom-radio-checkbox__show--radio"></span>
        <!-- Texto -->
        <span class="custom-radio-checkbox__text">{{nombre2}}</span>
      </label>
    </div>
  </div>
</template>
<script>
export default {
  props: ["nombre1", "nombre2"]
};
</script>

<style scoped>
label {
  font-size: 12px;
}
.custom-radio-checkbox__input span {
  border: 1px solid;
}

.radio {
  display: inline-flex;
  align-items: center;
}
.custom-radio-checkbox {
  display: inline-flex;
  align-items: center;
  cursor: pointer;
  font-family: arial;
  margin-right: 26px;
}

/* Modificador para dar la imagen de radio */
.custom-radio-checkbox__show--radio {
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
  padding: 5px;
  border: 0.1px solid black;
  border-radius: 50%;
}

/* Cambia el radio personalizado cuando es pulsado */
.custom-radio-checkbox
  > .custom-radio-checkbox__input:checked
  + .custom-radio-checkbox__show--radio {
  background-color: #fa2398;
}

/* Cambia el radio personalizado cuando es pulsado */
/* .custom-radio-checkbox
  > .custom-radio-checkbox__input:checked
  + .custom-radio-checkbox__show--radio {
  background-color: #fa2398;
} */
</style>